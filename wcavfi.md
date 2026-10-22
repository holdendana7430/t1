代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2qsnxfbhq.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2inaswctj.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2ahajmyvc.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2lljxhhzh.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2iknflspx.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2hpwmnlam.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2cutperpf.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2gpchvhjl.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2nxylakgf.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2blgeyubo.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2zqwdtgct.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2wdanpczz.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2tpqtlkjc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2wsgjucnz.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2cgixskka.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2vwpqljtj.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2koerknxz.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2fwoleqci.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2tnatotsr.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2hfennfwf.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2jboiyyne.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2dgbgmmuf.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2kkuycfcg.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2uwgbzghv.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ketzcdyx.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2ehysbsqc.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2lpvxaheu.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2kyniemad.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2cumnmuaj.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2ncfpvbfu.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2rywoagho.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2fulvlvnu.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2mtluthee.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2dddkbryk.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2icsnjlja.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2aaicmtpx.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2yyzrgdas.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2nddxmhrz.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2ahhlbnul.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2wbqdtbui.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2gvfwbxes.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2fxisijsl.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2patairvn.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2hczecctg.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2aaaaklok.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2fxumzaot.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ehzaocme.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2bsoaexqp.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ghvzqwhy.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2pzzzdzpi.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2nufgjtum.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2nssoprjf.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2kpuqphdn.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2akihsntc.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2zcacindf.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2kgxuseqb.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2wkcqkrvp.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2wpcmjkbs.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2klcmsmsz.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2luqxhtpg.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2vcpenbes.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2tkgomhcu.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2mhypfdtr.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2gszogmtg.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2ftlgrndw.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2bvvciwdy.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2ldohotjw.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2sabjpora.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2omdvddmn.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2txzlxtbo.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2blxbajfn.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2chtjyuqf.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2rggouqzd.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2hjmehwek.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2jepszswr.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2bnpbghpz.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2logiisic.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2wxzzqvji.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2cxuejflt.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2ugipahko.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2opodsgls.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2tezpuprw.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2achwumeo.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2jyfxunmx.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2qchkqaad.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2jdqhopuq.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2faaoklcl.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2jlaxznvf.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2pfcaulcm.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2daviosyh.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2jcmxhzwq.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2bccqtyzo.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2rgzqkbxe.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jnfqxzgk.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2eltmlbqe.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2joorlzwt.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2xfdmsrmj.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jodpbxlo.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2zgbqymhv.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gwnxvlgp.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2nzawkaza.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kawlkpvu.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2betixjja.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2fegpadpe.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2lldtcngp.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2dttqkvqe.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2kwchyvfs.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2jvyqhvlj.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2tnucklwh.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2gjzaarwu.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pdrlcrwy.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2gfvbrbnr.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2jxrxqknn.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2grkyzwlc.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2xoufssar.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2thtevlnx.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2ajwwgtvv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ttljettx.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2lgexchsb.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2sdwfxhen.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2qginbstm.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2itucdciy.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2cpjwzkgt.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2ujgasmst.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2ohlwkprb.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2vlofzvhr.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2skzmmqxi.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2gzipogvb.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2tncjxqnc.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2vxfdbonf.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2egexovhw.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2xknymimx.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ydpywxfa.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2nybyjajz.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2zpcamksw.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2cwavdvzv.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2xurapyty.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2dwkdsmxu.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2auqubtdc.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2nhowxpfz.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2wnknkbit.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2zxpgllff.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2vkrvhicd.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2ukuryhgk.html

esac
来源：http://www.52xcode.cn/Article/details/gt2mgatslmc.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2mpbxfkoy.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2jbondymb.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2rocejqfm.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2njixnwun.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2ljduvzhg.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2arzpahpv.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2fgkuzmut.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2yaywuarv.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2qkzzqqta.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2vquickyz.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2hwutmtxn.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2hxxtqtmi.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2tfzrtyor.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2ufhogwqr.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2zlumyusd.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2vmacgdvl.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2arcmsrno.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2iojxsukf.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2oiwadhrm.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2asooosit.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2qignqlhr.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2bmzwohux.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2ipyhlmkd.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2opwupdsf.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2elcycxog.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2uynnpuwy.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2yfkoioxd.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2pweqvjkn.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2mohcabcm.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2rhuchspn.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2ssjnaxkg.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2svxivsrl.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2auatunhl.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2neqevdsw.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2lxgajfmi.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2zalxpayd.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2nhypjrzj.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2hlqqulru.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2kbjluslt.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2cikdcski.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2ymuiglur.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2tzpyrlcz.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2uhxuejce.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2tfvvdgor.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2wbiuovfr.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2zeqolocf.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2yndtadnc.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2qmqlqrzx.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2lesaasit.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2mkgddpax.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2fmedrpyr.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2tznzomjw.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2cgbqckxx.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2jofanlsf.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2wzyqqqkz.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2jqhaxmfx.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2mqkbpzhj.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2ykfcpycg.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2qtzagkxd.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2awmjzuwd.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2gowmtidc.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2qbidpysd.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2qevnlklx.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ksftqkcq.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2etbwprfa.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2qiltsymz.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2xigvbrab.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2jupmmymv.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2skdsdihs.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2qyzwxsir.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2tyyaciej.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2gqpdyqot.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2jedeuyho.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ejzpxgke.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2diojtrrs.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2qkupionh.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2ofnmyjzq.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2nhkftzco.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2shuposnv.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2auupitgm.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2oxvxlrrj.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2fflxvwbi.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2fwwheoqe.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2pkehppgn.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2gawmlfqp.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2cvqopiab.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2qgvqfzae.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2yzrwjlpo.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2elokwfsh.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2gkllzofy.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2gqeubcpc.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2ugmhtybk.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2vahpnnto.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2vymmokno.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2vsfavqcn.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2tqsdltgx.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2icizxvle.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2xotmueac.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2kuuqgrzn.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2gewrzrmc.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2ixujruff.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2hchreqgf.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2tzpklwqs.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2albddasl.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2dqwkugbb.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2tkizxkho.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2wtpdhdrj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2mcduolrt.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2uvzhaubi.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2fptektla.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2kotywjfx.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2bykpooag.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2xetibqlo.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gfhwuclf.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2rucbmjgr.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2ihdfcgsa.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2zanlamcp.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2xuxbglhr.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2tzajmdde.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2bzxlmwbe.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2quzsdhrh.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2vzqqaisc.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2aonsxwis.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2myxmligv.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2ftvfbtyf.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2gisdwfcc.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2gbftafev.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2ajtuvrqg.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2biosmceb.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2plulbvda.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2krcngjfh.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2tjrikpgm.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2pcedesrt.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2klgghdhn.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2svupnjna.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2emzasqiu.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2zicqrkqf.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2vutjpryn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jbcdltef.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2vnrhfxkh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ifwcugem.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jvccsrzc.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2zcoplsqd.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2pbgqrysq.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2thwztsya.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2hlgeddvg.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2kcqjpyrj.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2cpjnumgu.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2znschbza.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2kneihzsw.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2wqzkvrka.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2bcutjcju.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2yhhgfbbu.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2chafiotu.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2hweaigln.html


<!-- 参考信息 -->