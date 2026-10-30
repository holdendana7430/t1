代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.fanxiaobao.xyz/Article/details/gjtpvlylh.sHtML

[Q54] 清空表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grmofzakr.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fanxiaobao.xyz/Article/details/gevwsbxkv.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fanxiaobao.xyz/Article/details/gxdcalsfd.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.fanxiaobao.xyz/Article/details/gyweuncmm.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gahlqruvx.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjqcjwma.sHtML

[Q57] 行号
来源：http://wap.fanxiaobao.xyz/Article/details/gmzshkvjq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvmnnpjpd.sHtML

[Q58] 累计求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gcxvqlpml.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/glihrtwxy.sHtML

[Q59] 分组内累计
来源：http://m.share.fanxiaobao.xyz/Article/details/gqpjxstio.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/giiycwbra.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvmcdywux.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fanxiaobao.xyz/Article/details/gwlsskglk.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gmuamqlsg.sHtML

[Q61] 移动平均
来源：http://mobile.fanxiaobao.xyz/Article/details/gxjqfihin.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/grxwlyckj.sHtML

[Q62] 分组占比
来源：http://read.share.fanxiaobao.xyz/Article/details/gfaklgvbq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdkannttx.sHtML

[Q63] 开启事务
来源：http://wap.fanxiaobao.xyz/Article/details/gruqbyxeu.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fanxiaobao.xyz/Article/details/glgaxcfnq.sHtML

[Q64] 提交事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsnclidju.sHtML

COMMIT;
来源：http://blog.fanxiaobao.xyz/Article/details/glhjqevjn.sHtML

[Q65] 回滚事务
来源：http://m.share.fanxiaobao.xyz/Article/details/ginjnnfiy.sHtML

ROLLBACK;
来源：http://wap.fanxiaobao.xyz/Article/details/grlgfluhp.sHtML

[Q66] 行锁查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmjlpkpa.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fanxiaobao.xyz/Article/details/gvzfbnhhp.sHtML

[Q67] 设置隔离级别
来源：http://baike.fanxiaobao.xyz/Article/details/gwigmqloe.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fanxiaobao.xyz/Article/details/glxgggqab.sHtML

[Q68] 保存点
来源：http://www.blog.fanxiaobao.xyz/Article/details/gerbrjoad.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giceokhhp.sHtML

ROLLBACK TO sp1;
来源：http://wap.fanxiaobao.xyz/Article/details/gopvjkzdp.sHtML

[Q69] 查看执行计划
来源：http://wap.fanxiaobao.xyz/Article/details/gdmehhpwd.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fanxiaobao.xyz/Article/details/gqevvnepf.sHtML

[Q70] 更新统计信息
来源：http://baike.fanxiaobao.xyz/Article/details/gjbrdntdu.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqpaftohh.sHtML

[Q71] 查看建表语句
来源：http://read.share.fanxiaobao.xyz/Article/details/gncsyvxwy.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fanxiaobao.xyz/Article/details/gpakvrvay.sHtML

[Q72] 查看索引
来源：http://3g.fanxiaobao.xyz/Article/details/ginxnjozb.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gldlguuwc.sHtML

[Q73] 查看表状态
来源：http://read.share.fanxiaobao.xyz/Article/details/ggviuyyfh.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/gixxktzyn.sHtML

[Q74] 强制使用索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gjikornvi.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fanxiaobao.xyz/Article/details/ggagfnloc.sHtML

[Q75] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gxeyuoluw.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnmvcuqfk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzqlrohck.sHtML

[Q76] 按天统计
来源：http://baike.fanxiaobao.xyz/Article/details/gnfqpurrk.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fanxiaobao.xyz/Article/details/gywinulxj.sHtML

[Q77] 时间加减
来源：http://blog.fanxiaobao.xyz/Article/details/gbxtebawi.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnikchqdf.sHtML

[Q78] 当前时间
来源：http://3g.fanxiaobao.xyz/Article/details/gywgmampn.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fanxiaobao.xyz/Article/details/gqjhaqpvn.sHtML

[Q79] 字符串拼接
来源：http://wap.fanxiaobao.xyz/Article/details/grlcmxbfj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtteltrd.sHtML

[Q80] 字符串截取
来源：http://read.share.fanxiaobao.xyz/Article/details/giwdfmphx.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gtxdcexxe.sHtML

[Q81] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gvbflqjby.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnvnguqll.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gigxnfjuv.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjjklcogu.sHtML

[Q83] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gnysnbsgn.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/grjpoohsl.sHtML

[Q84] 去除首尾空格
来源：http://wap.fanxiaobao.xyz/Article/details/gwaqionkk.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gjoefqktm.sHtML

[Q85] 数值取整
来源：http://wap.fanxiaobao.xyz/Article/details/grskijvwl.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fanxiaobao.xyz/Article/details/globlstvu.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fanxiaobao.xyz/Article/details/gzclsbfvn.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fanxiaobao.xyz/Article/details/ggooflytp.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gqexllpsl.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggfbrgimi.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.fanxiaobao.xyz/Article/details/gvlnnrjua.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fanxiaobao.xyz/Article/details/gcdvyfjcm.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gksqsnibc.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/givkdfivo.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gytkiudkd.sHtML

[Q90] 生成序号列
来源：http://3g.fanxiaobao.xyz/Article/details/gslcszeyo.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fanxiaobao.xyz/Article/details/gzxwoeqya.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gvsmydohd.sHtML

R. Bash 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gihphqlmj.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhomwuri.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fanxiaobao.xyz/Article/details/gchyoninl.sHtML

#!/usr/bin/env bash
来源：http://read.share.fanxiaobao.xyz/Article/details/gqtljttpo.sHtML

set -euo pipefail
来源：http://3g.fanxiaobao.xyz/Article/details/gnkcurlcs.sHtML

[R02] 变量赋值与使用
来源：http://3g.fanxiaobao.xyz/Article/details/gfvunoeuq.sHtML

name="Tom"; echo "$name"
来源：http://baike.fanxiaobao.xyz/Article/details/gbrxhbdvj.sHtML

[R03] 只读变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmcthamz.sHtML

readonly PI=3.14
来源：http://baike.fanxiaobao.xyz/Article/details/gxpmndubn.sHtML

[R04] 位置参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gzonhsmun.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fanxiaobao.xyz/Article/details/gwrmnmhkx.sHtML

[R05] 参数默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjfguawy.sHtML

name="${1:-default}"
来源：http://blog.fanxiaobao.xyz/Article/details/gkeqdgntx.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gwlgtaaki.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gsaazxftw.sHtML

[R07] if 判断文件
来源：http://wap.fanxiaobao.xyz/Article/details/guejfjtqe.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjgrcgyht.sHtML

[R08] 数值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnjortem.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfswqeonx.sHtML

[R09] 字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gofudtuxe.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gyhuugybj.sHtML

[R10] 正则匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gcfpcqzln.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwkdebxf.sHtML

[R11] case 多分支
来源：http://read.share.fanxiaobao.xyz/Article/details/gdcfwpyux.sHtML

case "$1" in
来源：http://blog.fanxiaobao.xyz/Article/details/gejjwfkbv.sHtML

start) echo "启动" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gqbpzlvgy.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxyjwtpfs.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggedqdbdq.sHtML

esac
来源：http://m.share.fanxiaobao.xyz/Article/details/gpiuwgwwu.sHtML

[R12] for 遍历文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gotwhajmz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfcumibqq.sHtML

[R13] for 计数循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gecssrbup.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmjvzxmbq.sHtML

[R14] C 风格 for
来源：http://baike.fanxiaobao.xyz/Article/details/gzvzstcgk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggdfanhoi.sHtML

[R15] while 逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gvrhfwkvb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqvgvouc.sHtML

[R16] until 等待条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gzmzrvzlo.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gnpfrravr.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatugwykb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gokknakvw.sHtML

[R18] 遍历数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gcqtnpqcf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvphpkkyo.sHtML

[R19] 数组长度
来源：http://m.share.fanxiaobao.xyz/Article/details/glgvfrsze.sHtML

echo "${#arr[@]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gswlgidfr.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fanxiaobao.xyz/Article/details/gkgevnlzw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gckdvtjwe.sHtML

[R21] 字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gbacyulqj.sHtML

echo "${#s}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzsbkekgy.sHtML

[R22] 截取子串
来源：http://read.share.fanxiaobao.xyz/Article/details/gzbrouluz.sHtML

echo "${s:0:5}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gcuuqjbpc.sHtML

[R23] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gfpiclqqa.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gqhyielqu.sHtML

[R24] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gpaapvhos.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gfqgazmub.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fanxiaobao.xyz/Article/details/gicpzzact.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fanxiaobao.xyz/Article/details/glahzwnyh.sHtML

[R26] 命令替换
来源：http://wap.fanxiaobao.xyz/Article/details/glvwhnhus.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fanxiaobao.xyz/Article/details/gjfgeywog.sHtML

[R27] 算术展开
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcpanojet.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fanxiaobao.xyz/Article/details/gvlaqsyoo.sHtML

[R28] 浮点运算
来源：http://blog.fanxiaobao.xyz/Article/details/gxyixuszn.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fanxiaobao.xyz/Article/details/gkqverhfz.sHtML

[R29] 定义函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gesnxkbik.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmcsryqif.sHtML

[R30] 函数返回状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gvrkgzzru.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fanxiaobao.xyz/Article/details/gnhsosaoe.sHtML

[R31] 局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/gevtvxidg.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwgvliqw.sHtML

[R32] 参数个数校验
来源：http://mobile.fanxiaobao.xyz/Article/details/gofdmrtmx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gudxzyaqb.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fanxiaobao.xyz/Article/details/gayeznyjh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fanxiaobao.xyz/Article/details/gsueervjd.sHtML

[R34] 退出时清理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxtteglsl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/ggsxndfpn.sHtML

[R35] 后台执行并等待
来源：http://baike.fanxiaobao.xyz/Article/details/gorxqckbz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glkmzklip.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdhxihek.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fanxiaobao.xyz/Article/details/gdsxcvkcs.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fanxiaobao.xyz/Article/details/grqvfhret.sHtML

files=$(ls -1)
来源：http://wap.fanxiaobao.xyz/Article/details/gdznrobwz.sHtML

[R38] 管道串联
来源：http://m.share.fanxiaobao.xyz/Article/details/gfnthomvx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gstmxcxae.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gltzzesrw.sHtML

cmd > out.log 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gweefhrhx.sHtML

[R40] 追加写日志
来源：http://baike.fanxiaobao.xyz/Article/details/gkywqzrgz.sHtML

echo "log" >> out.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaebfljua.sHtML

[R41] 丢弃输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gothoywxp.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gvlyceznb.sHtML

[R42] 输入重定向
来源：http://www.share.fanxiaobao.xyz/Article/details/gqxigqerr.sHtML

wc -l < a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/ggovykobq.sHtML

[R43] 按名字查找文件
来源：http://3g.fanxiaobao.xyz/Article/details/gnfzlexxt.sHtML

find . -name "*.log" -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/ghpbemdnn.sHtML

[R44] 按修改时间查找
来源：http://3g.fanxiaobao.xyz/Article/details/gvfozwzfh.sHtML

find . -mtime -7 -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gjhtnqxny.sHtML

[R45] 批量删除
来源：http://wap.fanxiaobao.xyz/Article/details/ggvdrgsqm.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fanxiaobao.xyz/Article/details/gepsglyax.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsztghtan.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fanxiaobao.xyz/Article/details/gmygqspxs.sHtML

[R47] sed 单行替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gjjstaajx.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gezxbotbi.sHtML

[R48] awk 取指定列
来源：http://3g.fanxiaobao.xyz/Article/details/gbuuniaes.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gvupwblus.sHtML

[R49] awk 带条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gowwgfucd.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/ggomfstvm.sHtML

[R50] awk 求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gudjgdqla.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gjwecvptn.sHtML

[R51] 排序去重取前几
来源：http://blog.fanxiaobao.xyz/Article/details/gdeorbwxr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fanxiaobao.xyz/Article/details/gbckhezwz.sHtML

[R52] 统计行数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjygzfqyx.sHtML

wc -l a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gqpmtnezy.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fanxiaobao.xyz/Article/details/ggxjcclbo.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gigkbvhhj.sHtML

[R54] 比较两个文件
来源：http://blog.fanxiaobao.xyz/Article/details/gxozsygnk.sHtML

diff a.txt b.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gqvelwvpb.sHtML

[R55] 压缩与解压
来源：http://m.share.fanxiaobao.xyz/Article/details/gdmqghfnx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fanxiaobao.xyz/Article/details/goxvsehwv.sHtML

[R56] 远程拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gtprbwkvv.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/gvkpmcszo.sHtML

[R57] 远程执行命令
来源：http://mobile.fanxiaobao.xyz/Article/details/gaolusiia.sHtML

ssh user@host 'uptime'
来源：http://mobile.fanxiaobao.xyz/Article/details/grwnastwb.sHtML

[R58] 下载文件
来源：http://wap.fanxiaobao.xyz/Article/details/gefextzsc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/gvqwyaqfe.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzugyllwh.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkgiakuhy.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gzvfnpuur.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fanxiaobao.xyz/Article/details/goduegtuy.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gahcsmxsj.sHtML

df -h;  du -sh *
来源：http://3g.fanxiaobao.xyz/Article/details/gkogusahu.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gbepplqzg.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcnleyfzm.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gqusprjks.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fanxiaobao.xyz/Article/details/gpqusimsx.sHtML

[R64] 结束进程
来源：http://wap.fanxiaobao.xyz/Article/details/gjspzthrp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdljpvmsd.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghtagxrik.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fanxiaobao.xyz/Article/details/gpodoseuf.sHtML

[R66] 定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwnwlcvo.sHtML

crontab -e;  crontab -l
来源：http://3g.fanxiaobao.xyz/Article/details/gmzvfkivv.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gambpaolf.sHtML

openssl rand -hex 16
来源：http://blog.fanxiaobao.xyz/Article/details/goxmflqnr.sHtML

[R68] 计算文件校验值
来源：http://m.share.fanxiaobao.xyz/Article/details/gjczjlrlm.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gukappspp.sHtML

[R69] 生成随机密码
来源：http://baike.fanxiaobao.xyz/Article/details/gmqficdod.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fanxiaobao.xyz/Article/details/gvkkbdktt.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbrohmgta.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fanxiaobao.xyz/Article/details/gdlqficyp.sHtML

[R71] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gnxkkphuo.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gebukluhi.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvkmedzx.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gsyyxcesu.sHtML

[R73] 分割大日志
来源：http://wap.fanxiaobao.xyz/Article/details/gcziihkgo.sHtML

split -l 1000 big.log part_
来源：http://blog.fanxiaobao.xyz/Article/details/gndmqadsr.sHtML

[R74] 批量重命名
来源：http://3g.fanxiaobao.xyz/Article/details/gvbjdxarz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gosqvlibl.sHtML

[R75] 导出环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gwebhfyrg.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fanxiaobao.xyz/Article/details/giylzqyhr.sHtML

[R76] 使用临时文件
来源：http://baike.fanxiaobao.xyz/Article/details/gouqcbvax.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gctqxeeoy.sHtML

[R77] 读取用户输入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gymktmuxx.sHtML

read -rp "请输入: " ans
来源：http://baike.fanxiaobao.xyz/Article/details/gvjfouvpo.sHtML

[R78] 交互式菜单
来源：http://baike.fanxiaobao.xyz/Article/details/gybcbiuul.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fanxiaobao.xyz/Article/details/gnusjokoq.sHtML

[R79] 解析命令行选项
来源：http://blog.fanxiaobao.xyz/Article/details/gdxmkpdex.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnqhynrps.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fanxiaobao.xyz/Article/details/gbflyqvqb.sHtML

time ./run.sh
来源：http://blog.fanxiaobao.xyz/Article/details/gjiuoyuwe.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gyoctpbaj.sHtML

S. C / C++ 专题
来源：http://3g.fanxiaobao.xyz/Article/details/grzcwpeaq.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gueqbqaqz.sHtML

[S01] C：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/ghghbwewn.sHtML

#include <stdio.h>
来源：http://www.share.fanxiaobao.xyz/Article/details/gpkwzlgnz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gojophodp.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/gcdabxknp.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gysiwjzyy.sHtML

[S03] C：读入整数
来源：http://baike.fanxiaobao.xyz/Article/details/gwurjxxxw.sHtML

int x; scanf("%d", &x);
来源：http://3g.fanxiaobao.xyz/Article/details/gyckniyzk.sHtML

[S04] C：字符串复制
来源：http://mobile.fanxiaobao.xyz/Article/details/gfqjdrmrc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtiirsono.sHtML

[S05] C：字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gblnbkzkg.sHtML

strlen(s)
来源：http://baike.fanxiaobao.xyz/Article/details/ggbpmwpif.sHtML

[S06] C：字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gbevphtew.sHtML

strcmp(a, b) == 0
来源：http://m.share.fanxiaobao.xyz/Article/details/gepisvsfv.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fanxiaobao.xyz/Article/details/goqaynaup.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fanxiaobao.xyz/Article/details/guafiyvxo.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxpywcvqc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fanxiaobao.xyz/Article/details/gbmheywbj.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fanxiaobao.xyz/Article/details/gpgwikazw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fanxiaobao.xyz/Article/details/gnhiekger.sHtML

[S10] C：指针与解引用
来源：http://3g.fanxiaobao.xyz/Article/details/gacrvhkiw.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfarnhhtu.sHtML

[S11] C：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gyzlzpksv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/gazirgojx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggdhcxtvn.sHtML

fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjjomtglb.sHtML

[S12] C：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzwvsjtat.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjveeasgo.sHtML

[S13] C：宏定义
来源：http://baike.fanxiaobao.xyz/Article/details/gshobtdei.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fanxiaobao.xyz/Article/details/gucvnfhrn.sHtML

[S14] C：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/grdosxgjh.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fanxiaobao.xyz/Article/details/gjkjtvgyo.sHtML

[S15] C：类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gzjxpfxsy.sHtML

(double) a / b
来源：http://blog.fanxiaobao.xyz/Article/details/ggwcuopcr.sHtML

[S16] C：位操作置位
来源：http://baike.fanxiaobao.xyz/Article/details/giaiyotej.sHtML

x |= (1 << 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gthqpehot.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gokbfffqb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gosthxmft.sHtML

[S18] C：命令行参数
来源：http://baike.fanxiaobao.xyz/Article/details/gjvwipqgh.sHtML

int main(int argc, char **argv)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpbidblhx.sHtML

[S19] C：快速排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glrcjkono.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gsyjfszhm.sHtML

[S20] C：二分查找
来源：http://www.share.fanxiaobao.xyz/Article/details/geptqbhhx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/glvslcaec.sHtML

[S21] C：字符类别判断
来源：http://wap.fanxiaobao.xyz/Article/details/gusntwifo.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fanxiaobao.xyz/Article/details/gphadnhnc.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gfoyyabfj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/gavgvkhjk.sHtML

[S23] C：随机数
来源：http://blog.fanxiaobao.xyz/Article/details/gwsgwqowz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/gboqzarir.sHtML

[S24] C：获取本地时间
来源：http://wap.fanxiaobao.xyz/Article/details/grspjunxw.sHtML


<!-- 参考信息 -->