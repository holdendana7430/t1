代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3yzyiujjy.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3qebaxseh.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3rhqyfred.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3vsbtyevi.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3gecpujao.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3fudsfzun.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3cqeicnob.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3lzoqpzug.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3denheghh.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3egccytmb.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3jenujwiw.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3kmvwxrzg.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3epsevzdz.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3iehzbsjk.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3qdczpzku.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3zinhtcrj.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3zmgzrnbs.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3lqhpvlps.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3pyippune.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3rxwhjkje.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3sdocssvy.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3yhtlisxp.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3beyvyjfb.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3ayrnlfho.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3skcuwgfk.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3cejlbhcz.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3iumaqopn.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3ajjaorho.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3mgrvlzfq.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3szrnqomw.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3bkkjfdov.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ydphiydo.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3wqqfoffw.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3epijxofh.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3gzssuijs.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3gbnwxrmd.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3hpnlxrph.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3jodluagx.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3odicajld.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3zvfagish.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3zllhtybq.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3nlzrzjsp.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3kneobeor.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3cnqrnyqn.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3qtugtwlj.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3iuyogyas.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3mcnmfibn.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3ywiwimsq.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3fwoshhwv.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3odinfexn.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3otlhmvkl.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3cslecatn.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3dticplda.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3sqidslkr.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3ziohovxy.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3ztulswnc.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3edlxolib.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3yucfeifi.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3jyqdwnqg.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3oaxlmxtg.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3rpsolsan.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3tjooekzs.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3dsrcavny.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3wmgmkkor.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3zxvivqzp.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3hdsthzvs.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3udhgggez.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3hexkeeyr.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3ijusybrp.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3fqcpdxgo.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3oigwspwk.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3dnrfjhll.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3wlvsgtbp.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hwsqdcgn.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3ertbfijp.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dftcvmun.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3wtrnkwrx.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fiwbfier.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3qnrrajic.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3huackvek.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3uepahhoj.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3eqwmdtlo.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3yupgxsjc.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3rhgplctv.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3sachqweh.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3pahalron.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3bclkpsaq.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3tqcaasth.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3wcftedun.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3gwfaeuvr.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hkuvvxdt.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3iwlvssim.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3bxncysej.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3wjrobzhw.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3uacrqcfq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pfbnjwcn.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3ozbyhbhb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lupywquc.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3yckuswrn.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3ssxjmvre.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3yxpurjnw.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3pcxblmgt.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3tuvgybxl.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3dkjwyqzc.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3jjwfvxld.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3zrpjtvuy.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3giafljlu.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3nxucopac.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3rilahxrd.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3jrrjlsxf.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3nusvutea.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3lowvrhrs.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3wfigcbdb.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3uxxfywyi.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3qpnruubh.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3leswwsea.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3xvvodaoy.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3qiqzdznk.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3bbtdxyee.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3ymejokfk.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3nepilmxx.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3iqutcqoc.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3acctklnm.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3bokqxspv.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3dbagfkfz.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3ipssyxkr.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3htzguopd.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3ogzrycnm.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3kfriygsq.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3diwwrrnt.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3zjctovpq.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3dfqgzzam.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3krjehqhr.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3goruxlss.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3bufeerth.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3obmkygxp.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3mbfiuroe.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3lksxyaik.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3mhexggmf.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3hnyfolgd.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3swiylkqg.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3yvyncrvc.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3vtjgrnby.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3ukgwsjav.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3brdxkvhx.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3qzbwkbrc.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3iurignul.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3knaofhfa.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3bzhdlsix.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ugwozmpq.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3blvwyaxb.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3xdmyikus.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3lseomxck.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3wagypmub.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3mjynhigh.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3hgqmswvx.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3fwfmztbo.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3yojjrbpl.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3rltndyrh.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3soameeqa.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3bgnookyg.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3xtnuqmmk.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3bztdoogg.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3smcwgwww.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3kpxrdntb.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3aquphgag.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3mgmtlehs.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3ijxuyqux.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3bxsyrlxa.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3dlfrywlj.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3dljdrdqs.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3kciifrrx.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3jcorvljc.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3ychrzrtn.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3uaivnsyo.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3trvfsogp.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3wadsnkbr.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3wjwkbcuu.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3biopnzse.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3lxdvtjxn.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3lnitwbxu.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3teqrymjc.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3mjwfnnpc.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3xvhivmzy.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3tztthevf.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3mtwavorr.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3ogyivslv.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3euvfmsxw.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3nisrdofl.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3uezuyimv.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3qjefbltp.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3aqydztrj.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3qgwvbrjr.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3stvophwh.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3tsrullou.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3xdbjsxqw.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3esextsbm.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3toltnrle.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zvfnslnh.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3kgabqcqq.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3cmlhqhjn.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3lzaivyrv.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3pszjpfeg.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3rfyqrvcf.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3rzcxafqb.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3njwgffwv.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3skenntlo.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3pnfthydy.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3nqttiovf.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3rjawgkvu.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tvubycoi.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3tuzfihmf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3ftmwhmjb.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3lzlmnayt.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3myelcmrb.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3wwidscrp.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3cbeqinnw.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3iwqvunhg.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3suuwrsur.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3wdurtkgl.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3szrfssfa.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3dufxfoka.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3tyzhuhrj.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3frtfxrgv.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3mdwymohq.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3mhpcyhgo.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3qvrxnosm.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3hqdhxcym.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3ccxckqtv.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3cbfznhpk.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3gpdsexqw.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3ygesjvxd.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3ddhywyxy.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3qwjalsct.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3yzzkkbpe.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3lzfgvkcl.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3tfvdhqdc.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3zraolacj.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wajbtdev.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3nvyxsniy.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3hdqqinlg.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3tinutlje.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3kyjbbhap.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3avpbiovm.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3gjrqovak.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3bjijgntm.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3avbhosub.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3jujzsozk.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3cpjnybqe.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3grvblcpn.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3wnfkzqpw.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3iwtanant.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3flifegrc.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3wrlfljiv.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3uuyqhuxp.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3krkpskjf.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3djrwcquq.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3ikxtnjok.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3tynrfjqg.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3gguhyikn.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3eujstjhm.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3dwytonxk.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3rbdklvvb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yzjsbswy.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3lzpnerlj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gxhvpalj.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jalznnjo.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3ynhfncet.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3cstgopfa.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3aduakncx.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3xamawjgc.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3nngdjwcw.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3uwnxcgsk.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3rksisclu.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3psbogorp.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3yoascenn.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3heensmqw.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3wcnsuxah.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3otsyqfst.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3asxrcmmh.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3gfytajbm.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3wwsedukm.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3bdvnoeja.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3lbuzestl.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3ewfvjmnz.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3hhrbgvud.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3carbaeic.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3blfeygod.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3nljvorfg.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3kyxkhbut.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3yyfogovf.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3eitakpsh.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3mlzccwic.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3omsomcet.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3mbifreem.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3buwlhusa.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3wiqqfpyu.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3lnxllrak.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3adlcuxao.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3arfzbopw.html


<!-- 参考信息 -->