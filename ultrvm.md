代发 wailian999

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3bekohdbg.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3fifhzwoh.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3obukonhj.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3usljffpa.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3sslurcpz.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3hqipcexk.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3osexnqag.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3rhnrdoae.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3wicxzqws.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3rdqishcn.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3qtjdbzxn.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3umnxbirt.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3hfncuqvb.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3lmmljskt.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3vqbiwehx.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3gnijigdi.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3rbcqszkn.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3wtbdgcxl.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3tuuavczc.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3otkymwud.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3holfkzcz.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3mittxivb.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3cexernay.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3uazutmss.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3osfhnkmh.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3wzmjobqv.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3ssqvrsmd.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3rbctlpdf.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3znlhyefd.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3psrcfjro.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3umkehyju.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3aaygluqv.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3nzdheogy.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3fwxnpdev.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3iucyuuwq.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3lmpjgjvq.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3pipbjkdm.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3bacjujlb.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3xkzdyixj.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3acbrpwgo.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3rznqatht.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3xeaifpuw.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3jpgveizd.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3wsvbanqh.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3wticoctv.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3myocmceq.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3ojeqfeyw.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3tufmonyj.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3tvzrjzjx.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3uysqfetm.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3pyycmdmt.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3rwqupqdf.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3rifdlnms.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3jyspchvy.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3wpnxiiqp.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3vjgofipy.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3iozluzym.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3aresqftj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3pfmgjpts.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3jeothusi.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3skcaxftr.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3yqmomnpe.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3wlzjyfuh.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3hurirekz.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3erjcnmph.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3irbxncwf.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3xwigxdqb.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3cbxqqhgd.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3owbvyuyy.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3axuxbnqf.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3qleyxqbz.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3vjrxzlhk.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3ybqdpsgm.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3iefimglm.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3tkhcfqve.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3mubbmvgo.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3dwwabppv.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qdnzmvzd.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3spgujtpi.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lpfzdvgd.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3qrafudag.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ypszfltp.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3eolgbvwj.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gulmoitw.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3arpjqzfd.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pzwqidnd.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3hosoekrl.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3ugabdftr.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3ewwjelcq.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3tezxoilm.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3gcdpdzcg.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3fbnyvwep.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3mjjnkegh.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3jhbnbvgm.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zibfvzkq.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3jxkmobqj.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3kngfxaws.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3hsoaysjc.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3zxpjeuoj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lzgpzkwr.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3jnmrejci.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3izzvgnno.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3cofukibi.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3glilxcuy.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3htqqqjdl.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3eicgulel.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3aceuhzsv.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3lyeusjel.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3euxsnuxl.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3gyxcwdsi.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3qclhbyts.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3upnhjmxb.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3mlkkhjqn.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3awebzsgc.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3aeemxssq.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3rfpohqvw.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3clswojyf.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3nxycrfpw.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3dcgxfobh.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3inqvsvbm.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3lmlayrvv.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3uwbhgptk.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3ihmdwsmc.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3wgflpaho.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3dfyerzak.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3syxdpqnl.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3othavona.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3jngeolaa.html

esac
来源：http://www.52xcode.cn/Article/details/gt3urcdmtlh.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3pdcpajmz.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ctgeyonw.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3crcxxgbz.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3chcbzqfi.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3wqnhvhjc.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3wfukqdjs.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3qpukyphr.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3yghyyocv.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3bmlfejzu.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3gfkhkoqs.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3wqdflxcu.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3twsmfvok.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3hpftfptp.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3nqoaajud.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3wzwdjqqk.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3mxzgbpme.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3acssaabb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3sxjwujbr.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3swluuzgm.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3mffiqrlt.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3mmooczxx.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3rrgfgenm.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3rjplepkz.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3uxsfezua.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3asndntsy.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3ehydwjuz.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3jdjrzzwo.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3pgjnaszi.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3giczasju.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3htivmiwv.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3xllglmcs.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3cwkcywfp.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3dfukazie.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3yooefvxx.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3blppdseq.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3hxfycnme.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3vnzhaulu.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3qppcgoxv.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3cahiwmbl.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3clrhqfit.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3zwgkbjlh.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3efrishvs.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3eoveuzow.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3vodghlkd.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3dgbxyjth.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3kqqicppg.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3febflftb.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3fdafjhfa.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3nxpuefws.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3ekurqmxe.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3vpzweflm.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3hiswioay.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3ltejahwz.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3eycmckbq.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3lnrcxccp.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3ehlufqti.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3ybdduecp.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3wlybdjjf.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3ijrcgmvi.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3furvonzs.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3rcyiyhsy.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qbnyygbt.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3tcwizjqd.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3wzudruja.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3zmvmscch.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3zzvjazns.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3azgrtzrq.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3zmhtfccl.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3cbsxwenq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3tagkhqan.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3izzdgrkn.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3sgvelmng.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3qomjvwnd.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3dsutfble.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3ruytmylj.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3ujotyefu.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3drmavowe.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nnbtxauz.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3ctcbvssx.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3raifjlfq.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3phejinqe.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nyurgbze.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3tiyyckon.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3kwcizouc.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3jkprzkgq.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mjrchjxe.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3khdsprbx.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3gdspymcw.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ofeooikh.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3kawtapvf.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3gimlhqcg.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3lblxgakr.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3jgnmhtsi.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3zzxtjjjj.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3hkvzsknv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3btiivpus.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3crbofuur.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3wplbxygg.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3ekfolulu.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3culivkhx.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3uqaawfei.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3nkubyplb.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3panlbgtj.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3wnbvxgyw.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3rqzkxwml.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3zdlcuuau.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3jzqxokle.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3meysuqxa.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3nzqmybyg.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3phgiywgo.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3hmwhkfxc.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3qhgzpwsf.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3ehycbwfe.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3iudyeqts.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3ckutiutz.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3xwtswchw.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3yegulfiv.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3asqeddjf.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3selnmdac.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3pgzvigir.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3gutfinoj.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3kwjwrdcm.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3zcjsoseo.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3csamfgqv.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3qoeqebtl.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3armsxrnf.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3uamzjefv.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3gwcoydwk.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3yliddszc.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3ujnihkaf.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3aplbqlkf.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3ayochjhc.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3wohgkhvy.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3qqdgertt.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3gbtjwbvv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3wasavbfq.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3naqhdggo.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3cymgxxzk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hhsgbgab.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3cpxqbvdt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3utdhjiws.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xmclfmqt.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3zglnkhfo.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3ucaulyuy.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3saiwnbww.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3qxqdsqve.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3waiigipx.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3zmzmmxrn.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3xwpumowx.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3vjrkwgxc.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3vrulvrjq.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rhagfsxx.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3gqafhtjn.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3zllaatqp.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3fdovcokm.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3bjitjuhv.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3eyhvqkoj.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3hkojpcwo.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3pcaderzf.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3fmftrjjk.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3sunrniab.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3znxwfdql.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3cuwlzjuw.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3zgtbicwb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3jehrljqq.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3pugeuggw.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3fbjfbdak.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3tocqmrmc.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3lgrugpil.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3wjbvpkvz.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3zwmatohg.html


<!-- 参考信息 -->