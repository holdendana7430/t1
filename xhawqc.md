代发 wailian999

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2ufjnngmd.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2yharjfey.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2hhlbeeru.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2fexzpuhq.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2zfgcacxx.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2wgkpfgji.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2jpfrlemo.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2wdsbebfl.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2xrxiljqe.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2iybjbmid.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2nglomach.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2vmjbaxyf.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2tvgcrdso.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2tlbhpdhs.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2fdlgkwhy.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2jdtixxus.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2afbmcvgl.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2xvzgmoak.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2qpyspywp.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2xlbwapce.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2oqficbfc.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2krpdhjad.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2juoklzwv.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2wikccehw.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2vnxvliaw.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2xvwmqaec.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2szpnnreh.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2cizsiidy.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2drbvbugs.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2jjhbylrx.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2dduvfdui.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2ohmfwjtn.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2dasbtzes.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2douqlbcs.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2ntjgokpi.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2gyjhsjbj.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2ypyvmgvs.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2thiltmra.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2xloxtuvi.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2rhdmrtri.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2mbseufwg.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2gezcxjlx.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2cmiulqom.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2shepnfvj.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2ienlpbke.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2jeimstri.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2tjmbcovw.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2hnymxoqx.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2ncymdttk.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2tgdxcslq.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2rgehfhus.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2camwbhpz.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2iitdyryv.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2hxiulaqq.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2gixwuugz.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2bakcsyxj.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2jrlwhxdn.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2klvujzdg.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2wsuaurfw.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2hvatlfuv.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ggcqikpr.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2aushlziq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2nuydlvhq.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2loayocmq.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2unsqsblo.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2fmxotlmi.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2viivpdkn.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2tohqbfkv.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2yuuotptb.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2qdvcmwkl.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2rgilshpp.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2ztaztxsl.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2mtcvlqwd.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2qxuwgbhl.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2kzxpxjds.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2evttfudx.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2qsitqiey.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kfeduzgd.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2vglswnne.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2iurgvvou.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2snqnvoeb.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ysfbrfnc.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2xyeryohs.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2opgpbocz.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2mrvishaf.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zncciyoy.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2fhrkxjnu.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2xitbzmke.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2rcbkmdfj.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2bifsifog.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2vgmtekqn.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2fvcjesjp.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2oocwnwnf.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2iaecmtfi.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dwtfnmpz.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2owmagwsk.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2lnogyfvn.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2yylvtriu.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2oxxjfdod.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kaqkhmol.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2jjwnbsgv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rhqirnaw.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2ohrctswd.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2aexfmhta.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2bjbfsida.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2dhwouzwl.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2ezslpvyk.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2owdiikqb.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2gvxprfft.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2mnhjrlsj.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2djwofssz.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2ydmaesxd.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2brzvkrdy.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2wcwycrxs.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2tbjuhdri.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2pazpjjeu.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2pghtxxvx.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2qtdixufy.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2libbvzqp.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ugcvceam.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ubxzfrgu.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2bujgbopl.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ylnpgvkw.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2pflkicek.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2oztgisrf.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2bhoomhqe.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ifqjpuef.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2xbvufyml.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2macnqvay.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2pymzffqe.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2vgiymnrh.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2swdyumgs.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ljdyjvdt.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2rfsxuokj.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2tclwbwlg.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2eabzcsei.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mipxymwr.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2ggrpnomr.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2daojepxy.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2iimizwsi.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2sdrsxlho.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2morxfxqo.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2msujwzuo.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2vmpbzgzj.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2vqyheyyl.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2gludrthr.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2hxaaohtz.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2nwdtiyqo.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2muxrjqdv.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2zicumyya.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2yihdbhet.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2fzuefubu.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2wosboygc.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2noirlvrt.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2wxkzeiem.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2lgoekblp.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2jkqskyyb.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2oupivgim.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2ulipuyel.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2pplejcij.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2nahvjgua.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2eigoisoi.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2cswaejvo.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2kwggnfnr.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2vgnzgmpg.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2scynothj.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2jnrsrygc.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2jxmgnqeg.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2veyibxyx.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2wyagbxzd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2zhexpfbr.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2uyouhlkn.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2vqkfmbjg.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2ftwapozv.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2gfqphxyq.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2yhgcjpjq.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2ichqmgjw.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2bvgbfnmh.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2imkrrlxy.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2dznwmknl.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2kxozaaok.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2lqcbnnic.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2pxbjnddi.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2uynsbjwq.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2ktnxldch.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2gmiaayce.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2wgwnxdmu.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2ioojigav.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2fwrcpkrt.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2wotxyvko.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2npskzhru.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2phhkzuvi.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ewtiwpqz.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2yefqzblt.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2tmxzsrsa.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2mdesulqa.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2fdfdyhqd.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2yezmvame.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2tahamlyc.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2ljhvfivg.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2xadcxoyo.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2hyygeulg.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2iisvlglt.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2renyscbu.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2gxxdzgej.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2kkzhtjnp.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hvlxooqv.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2jwlnkpzm.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2gfyboopv.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2mfmwcrig.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2nylureww.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2ybiogsqx.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2xojtofng.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2ogbfdsrz.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2sgeeefkv.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2ouwxwjvr.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2cfatmmgf.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2gatgicxc.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2iphhtrmu.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2snbwsalr.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2aronzdlj.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2eakxjced.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2wjeiohkv.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2xfgrkkbb.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2mdfcbufz.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2vopcugky.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2pmrhzjra.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2rryihidx.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2dbcmsywf.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2yhbkasdn.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2xigcmstd.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2lwbkchbz.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2ipxwaohy.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2gpgavvkf.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2zauxtmmj.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2biwjgtln.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2qnxzimfz.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2xzjhmrww.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2ijpslbqi.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2dgdowbrr.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2qylvaact.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2mqbiwoma.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2cgxoddvn.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2vcldtjxn.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2rqferlao.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2acdudmrq.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2rxwfdldm.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ndbrlqmj.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2zsxwdice.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2lanvixnq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2rukklfqy.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2bftpnnmk.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2fcxuseqq.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2klshmcuw.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2gaobfpel.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2xjyczsxy.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2xhknhomy.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2nvjevvvw.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2uimwbkjy.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2eqxizyse.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2hpzyamhp.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2plakjxdi.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2ziqlurqy.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2duvhreio.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2hcniwpis.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2scpwgbnr.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2flmvzbrk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qcmalsbd.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2wfzyubus.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kohdcigs.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2uizudpem.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2phigouig.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2ejfqveno.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2sizrjpoi.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2ldauecwn.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2rsycofsf.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2wwygzzfq.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2uxorbycm.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2xuyaeuxo.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2pgosxqzd.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zhjreimd.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2zkrkhgeo.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2kbyhcjma.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2wwhqvuxk.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2qkykphza.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2nebtoxvm.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2xwzxbrqh.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2frhhcmiq.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2tzshcyok.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2wtmxugvr.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2hvfgffvd.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ktpvotot.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2phouxuyx.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2uhxeufst.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2pkbjljdn.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2rawxecds.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2ptrqpmop.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2fnnbxuyz.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2hjqkfqnd.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2lkobykpp.html


<!-- 参考信息 -->