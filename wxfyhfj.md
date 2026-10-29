代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.zdbjq.cn/Article/details/gbryrriim.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/gbxpvhrxw.sHtML

[Q47] 与平均值比较
来源：http://mobile.zdbjq.cn/Article/details/gdlnumuvg.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fehbvm.com/Article/details/gptvfwyrr.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fehbvm.com/Article/details/gxuqnshqp.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fehbvm.com/Article/details/gwcvrmrhj.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.hesvh.cn/Article/details/gwjbezrdd.sHtML

[Q49] 更新单行
来源：http://www.share.hesvh.cn/Article/details/gnevynepf.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/gkcctsdsx.sHtML

[Q50] 批量更新
来源：http://wap.fehbvm.com/Article/details/gfeskoxyl.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.fehbvm.com/Article/details/ghmampire.sHtML

[Q51] 用子查询更新
来源：http://www.blog.zdbjq.cn/Article/details/guukxpzmx.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.hesvh.cn/Article/details/gvgzfvtrj.sHtML

[Q52] 删除指定行
来源：http://www.m.share.zdbjq.cn/Article/details/gerzqcuop.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/gbtyccijo.sHtML

[Q53] 按条件删除
来源：http://m.share.fehbvm.com/Article/details/geinuxzcc.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.zdbjq.cn/Article/details/gqtoyfpca.sHtML

[Q54] 清空表
来源：http://3g.fehbvm.com/Article/details/gwgchtkqi.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fehbvm.com/Article/details/gellxzjnt.sHtML

[Q55] 排名（并列占位）
来源：http://wap.zdbjq.cn/Article/details/glnihoaou.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/gndwrejiy.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.zdbjq.cn/Article/details/gbqvtoqih.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.zdbjq.cn/Article/details/gzxblpflq.sHtML

[Q57] 行号
来源：http://mobile.hesvh.cn/Article/details/gdolltdnq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gpkidbywv.sHtML

[Q58] 累计求和
来源：http://blog.zdbjq.cn/Article/details/gqqralruz.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.hesvh.cn/Article/details/glrauntuz.sHtML

[Q59] 分组内累计
来源：http://baike.fehbvm.com/Article/details/gyhzuoxcb.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/geigoiojl.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.hesvh.cn/Article/details/gtgldddcx.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.zdbjq.cn/Article/details/glzusdhby.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gctazkrgw.sHtML

[Q61] 移动平均
来源：http://m.share.zdbjq.cn/Article/details/gdbcalamw.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gdzxjnjhi.sHtML

[Q62] 分组占比
来源：http://m.share.fehbvm.com/Article/details/ghalphavj.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/ggpmjdtot.sHtML

[Q63] 开启事务
来源：http://www.blog.fehbvm.com/Article/details/gaghqmdcz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.zdbjq.cn/Article/details/gtpocayje.sHtML

[Q64] 提交事务
来源：http://baike.hesvh.cn/Article/details/gglanczlm.sHtML

COMMIT;
来源：http://www.m.share.hesvh.cn/Article/details/gikqwpvmp.sHtML

[Q65] 回滚事务
来源：http://blog.fehbvm.com/Article/details/gvxbapkjd.sHtML

ROLLBACK;
来源：http://blog.fehbvm.com/Article/details/gobgsylkq.sHtML

[Q66] 行锁查询
来源：http://mobile.zdbjq.cn/Article/details/gdytmzbls.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fehbvm.com/Article/details/gqdxbznhd.sHtML

[Q67] 设置隔离级别
来源：http://www.share.hesvh.cn/Article/details/gonussfjg.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.zdbjq.cn/Article/details/gbfiynphu.sHtML

[Q68] 保存点
来源：http://baike.fehbvm.com/Article/details/gdzxltwjw.sHtML

SAVEPOINT sp1;
来源：http://wap.fehbvm.com/Article/details/gssbzssse.sHtML

ROLLBACK TO sp1;
来源：http://mobile.hesvh.cn/Article/details/gsfnjmuua.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.zdbjq.cn/Article/details/gevnisczo.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fehbvm.com/Article/details/gihyfzwdz.sHtML

[Q70] 更新统计信息
来源：http://blog.hesvh.cn/Article/details/gtglbemgk.sHtML

ANALYZE TABLE users;
来源：http://www.blog.zdbjq.cn/Article/details/gnenwgtjw.sHtML

[Q71] 查看建表语句
来源：http://read.share.hesvh.cn/Article/details/gjeorehds.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.zdbjq.cn/Article/details/ghrwhaqwt.sHtML

[Q72] 查看索引
来源：http://read.share.hesvh.cn/Article/details/gypudldlf.sHtML

SHOW INDEX FROM users;
来源：http://baike.fehbvm.com/Article/details/gpwsdekhw.sHtML

[Q73] 查看表状态
来源：http://www.blog.hesvh.cn/Article/details/grokuwqqk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/gszrgbrjv.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fehbvm.com/Article/details/gdfzlqhlb.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.fehbvm.com/Article/details/gemyrnnnl.sHtML

[Q75] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gnizopctk.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gulkgzzly.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.zdbjq.cn/Article/details/gybltosnt.sHtML

[Q76] 按天统计
来源：http://mobile.fehbvm.com/Article/details/gxbfhumri.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fehbvm.com/Article/details/gcbqwkios.sHtML

[Q77] 时间加减
来源：http://3g.fehbvm.com/Article/details/gxztfrxeb.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fehbvm.com/Article/details/gpqakmpxc.sHtML

[Q78] 当前时间
来源：http://blog.fehbvm.com/Article/details/gxlogyjdf.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fehbvm.com/Article/details/gvigsnhpa.sHtML

[Q79] 字符串拼接
来源：http://m.share.fehbvm.com/Article/details/greuadmnk.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.hesvh.cn/Article/details/gtjqhuglr.sHtML

[Q80] 字符串截取
来源：http://baike.fehbvm.com/Article/details/givvsnqcu.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gbnxsstqn.sHtML

[Q81] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gxvvrhlbd.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.hesvh.cn/Article/details/gdvaduefs.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fehbvm.com/Article/details/gyoxifpia.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/glwuibryx.sHtML

[Q83] 大小写转换
来源：http://blog.fehbvm.com/Article/details/gqfvcakri.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gvncdwnsi.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fehbvm.com/Article/details/grfrgnlpq.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gqizuowgw.sHtML

[Q85] 数值取整
来源：http://www.share.fehbvm.com/Article/details/gvaaikkul.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fehbvm.com/Article/details/gkeotxnmd.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fehbvm.com/Article/details/gavlvivbs.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.hesvh.cn/Article/details/gfgovqgid.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fehbvm.com/Article/details/gswujlmgp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fehbvm.com/Article/details/gzjdxdahp.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fehbvm.com/Article/details/gxulhyxyt.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.hesvh.cn/Article/details/gcfpzdonr.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fehbvm.com/Article/details/gdgexstuo.sHtML

[Q89] 判断表是否存在
来源：http://blog.fehbvm.com/Article/details/gzkirxgps.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.zdbjq.cn/Article/details/gnaksrhdm.sHtML

[Q90] 生成序号列
来源：http://3g.zdbjq.cn/Article/details/gcgqtxruy.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.hesvh.cn/Article/details/glucwvidp.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gsrnmrkpe.sHtML

R. Bash 专题
来源：http://m.share.fehbvm.com/Article/details/gqoimyihi.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gfhsdgejv.sHtML

[R01] shebang 与严格模式
来源：http://wap.hesvh.cn/Article/details/guxfavpze.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fehbvm.com/Article/details/gdofuytqz.sHtML

set -euo pipefail
来源：http://blog.zdbjq.cn/Article/details/gfonzfdbb.sHtML

[R02] 变量赋值与使用
来源：http://mobile.hesvh.cn/Article/details/ghedunvcm.sHtML

name="Tom"; echo "$name"
来源：http://3g.fehbvm.com/Article/details/gtncbywiz.sHtML

[R03] 只读变量
来源：http://baike.hesvh.cn/Article/details/guesgtgsf.sHtML

readonly PI=3.14
来源：http://www.blog.hesvh.cn/Article/details/gkikkyqrw.sHtML

[R04] 位置参数
来源：http://baike.fehbvm.com/Article/details/ginjgtzvs.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fehbvm.com/Article/details/gnhbdgnhw.sHtML

[R05] 参数默认值
来源：http://mobile.zdbjq.cn/Article/details/gvkxqiqwx.sHtML

name="${1:-default}"
来源：http://blog.fehbvm.com/Article/details/gwvaqmdfa.sHtML

[R06] 判断命令是否存在
来源：http://read.share.hesvh.cn/Article/details/gzzzheikj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gyblxzvmb.sHtML

[R07] if 判断文件
来源：http://m.share.fehbvm.com/Article/details/gyqvpzzip.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.hesvh.cn/Article/details/gmczcujwc.sHtML

[R08] 数值比较
来源：http://3g.hesvh.cn/Article/details/gmzsbraye.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.zdbjq.cn/Article/details/guhehtpjg.sHtML

[R09] 字符串比较
来源：http://3g.hesvh.cn/Article/details/gvfstkywo.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fehbvm.com/Article/details/gveqckpxi.sHtML

[R10] 正则匹配
来源：http://www.blog.zdbjq.cn/Article/details/gapnkyrhp.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.zdbjq.cn/Article/details/gbrsqjpuu.sHtML

[R11] case 多分支
来源：http://baike.fehbvm.com/Article/details/gghvfnxru.sHtML

case "$1" in
来源：http://www.blog.hesvh.cn/Article/details/gaxhcaqli.sHtML

start) echo "启动" ;;
来源：http://wap.hesvh.cn/Article/details/gwqbmfnzh.sHtML

stop)  echo "停止" ;;
来源：http://blog.fehbvm.com/Article/details/gbjphegai.sHtML

*)     echo "未知命令" ;;
来源：http://baike.zdbjq.cn/Article/details/gmmzcpvei.sHtML

esac
来源：http://www.m.share.zdbjq.cn/Article/details/gpfjvatte.sHtML

[R12] for 遍历文件
来源：http://m.share.hesvh.cn/Article/details/gyqhonimr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.hesvh.cn/Article/details/gkqridlfm.sHtML

[R13] for 计数循环
来源：http://baike.hesvh.cn/Article/details/gztabbknq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fehbvm.com/Article/details/geskwbnea.sHtML

[R14] C 风格 for
来源：http://3g.fehbvm.com/Article/details/gshgttuvr.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/ghsjaljyw.sHtML

[R15] while 逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gmwfgsdrc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.hesvh.cn/Article/details/glnflmsrw.sHtML

[R16] until 等待条件
来源：http://3g.hesvh.cn/Article/details/gxdquciqi.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/gwvnmrfbs.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.hesvh.cn/Article/details/gvozrfvzf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.hesvh.cn/Article/details/gfrrtnwzb.sHtML

[R18] 遍历数组
来源：http://www.blog.hesvh.cn/Article/details/gahrkrfgg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.zdbjq.cn/Article/details/gzafgrsfh.sHtML

[R19] 数组长度
来源：http://wap.fehbvm.com/Article/details/golpqwuvl.sHtML

echo "${#arr[@]}"
来源：http://mobile.fehbvm.com/Article/details/ghngoyffx.sHtML

[R20] 关联数组（字典）
来源：http://blog.hesvh.cn/Article/details/gupwvxhyf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.hesvh.cn/Article/details/gtxwlxigf.sHtML

[R21] 字符串长度
来源：http://3g.zdbjq.cn/Article/details/gdhnciifl.sHtML

echo "${#s}"
来源：http://read.share.hesvh.cn/Article/details/gxkwpmpxv.sHtML

[R22] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/giszwdgxn.sHtML

echo "${s:0:5}"
来源：http://blog.zdbjq.cn/Article/details/gocceqknc.sHtML

[R23] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/gmdsdjaji.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.zdbjq.cn/Article/details/goxpxdnhq.sHtML

[R24] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gxmsgcfme.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.hesvh.cn/Article/details/gwzthzapn.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fehbvm.com/Article/details/gmznlemxl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.hesvh.cn/Article/details/gtnvdrsju.sHtML

[R26] 命令替换
来源：http://www.share.hesvh.cn/Article/details/ghlhuyxze.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fehbvm.com/Article/details/gsibylgcr.sHtML

[R27] 算术展开
来源：http://www.blog.hesvh.cn/Article/details/gdbdytghc.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.hesvh.cn/Article/details/gvoctnsfn.sHtML

[R28] 浮点运算
来源：http://m.share.zdbjq.cn/Article/details/gxuaxagnp.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.zdbjq.cn/Article/details/gmtldqdml.sHtML

[R29] 定义函数
来源：http://www.m.share.hesvh.cn/Article/details/gnzzqkhmy.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.zdbjq.cn/Article/details/gbwfxigbq.sHtML

[R30] 函数返回状态码
来源：http://m.share.zdbjq.cn/Article/details/gcnoomikg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.zdbjq.cn/Article/details/gfywhwrko.sHtML

[R31] 局部变量
来源：http://mobile.zdbjq.cn/Article/details/gmzozcmpr.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.hesvh.cn/Article/details/gxhxbbmkb.sHtML

[R32] 参数个数校验
来源：http://www.share.fehbvm.com/Article/details/gpbrtgvuh.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/gmgucxjqw.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.hesvh.cn/Article/details/gfkrxtsxj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fehbvm.com/Article/details/gzrkqdlnp.sHtML

[R34] 退出时清理
来源：http://3g.fehbvm.com/Article/details/gymhhxyok.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gargsqsxk.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.zdbjq.cn/Article/details/gaifelads.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fehbvm.com/Article/details/gsiuzfxel.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fehbvm.com/Article/details/gigswzybh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.zdbjq.cn/Article/details/gspuakpum.sHtML

[R37] 把输出赋给变量
来源：http://mobile.hesvh.cn/Article/details/gjivcqzct.sHtML

files=$(ls -1)
来源：http://www.blog.fehbvm.com/Article/details/gwmsussdm.sHtML

[R38] 管道串联
来源：http://baike.hesvh.cn/Article/details/gmksgfcdk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fehbvm.com/Article/details/glroossti.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.zdbjq.cn/Article/details/gqrhgjvll.sHtML

cmd > out.log 2>&1
来源：http://mobile.fehbvm.com/Article/details/gwmjpnysj.sHtML

[R40] 追加写日志
来源：http://mobile.fehbvm.com/Article/details/gxheapctj.sHtML

echo "log" >> out.log
来源：http://www.share.zdbjq.cn/Article/details/gbqhogxxi.sHtML

[R41] 丢弃输出
来源：http://wap.hesvh.cn/Article/details/galbhruai.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.hesvh.cn/Article/details/gifmybnae.sHtML

[R42] 输入重定向
来源：http://www.share.zdbjq.cn/Article/details/gvibkzsse.sHtML

wc -l < a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gohrteanw.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.hesvh.cn/Article/details/gnrfrjgvn.sHtML

find . -name "*.log" -type f
来源：http://mobile.zdbjq.cn/Article/details/gwjeaetvz.sHtML

[R44] 按修改时间查找
来源：http://mobile.zdbjq.cn/Article/details/gwkcilmxb.sHtML

find . -mtime -7 -type f
来源：http://www.blog.hesvh.cn/Article/details/gnurghgvz.sHtML

[R45] 批量删除
来源：http://3g.hesvh.cn/Article/details/gjomaylig.sHtML

find . -name "*.tmp" -delete
来源：http://baike.hesvh.cn/Article/details/gxeddnzge.sHtML

[R46] 递归替换文件内容
来源：http://m.share.hesvh.cn/Article/details/gnwapdvja.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.zdbjq.cn/Article/details/gllrtcawi.sHtML

[R47] sed 单行替换
来源：http://mobile.zdbjq.cn/Article/details/gjxnqltjd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fehbvm.com/Article/details/gnwvuwjsm.sHtML

[R48] awk 取指定列
来源：http://read.share.hesvh.cn/Article/details/gjtlqixcn.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gqivlxuxb.sHtML

[R49] awk 带条件
来源：http://wap.fehbvm.com/Article/details/guqqlfxmb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.zdbjq.cn/Article/details/gnhspswiy.sHtML

[R50] awk 求和
来源：http://baike.fehbvm.com/Article/details/gzsjdeiwk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fehbvm.com/Article/details/guvxpbwmt.sHtML

[R51] 排序去重取前几
来源：http://wap.fehbvm.com/Article/details/gmsjsspfk.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.zdbjq.cn/Article/details/gtjemgpqa.sHtML

[R52] 统计行数
来源：http://baike.fehbvm.com/Article/details/gxsgqqvzk.sHtML

wc -l a.txt
来源：http://3g.hesvh.cn/Article/details/gpdaokwet.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.zdbjq.cn/Article/details/geemzawcz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.zdbjq.cn/Article/details/gjctnykbz.sHtML

[R54] 比较两个文件
来源：http://www.blog.fehbvm.com/Article/details/grfrcetzc.sHtML

diff a.txt b.txt
来源：http://baike.hesvh.cn/Article/details/gqdtxmxum.sHtML

[R55] 压缩与解压
来源：http://blog.fehbvm.com/Article/details/gsaxikuzm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.zdbjq.cn/Article/details/gqtoupxyq.sHtML

[R56] 远程拷贝
来源：http://mobile.zdbjq.cn/Article/details/gwvkabgtc.sHtML

scp file user@host:/path/
来源：http://read.share.hesvh.cn/Article/details/guilvzqcm.sHtML

[R57] 远程执行命令
来源：http://3g.hesvh.cn/Article/details/gbivgaahv.sHtML

ssh user@host 'uptime'
来源：http://mobile.zdbjq.cn/Article/details/gyjodbutv.sHtML

[R58] 下载文件
来源：http://m.share.hesvh.cn/Article/details/gawumqzho.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.zdbjq.cn/Article/details/gmkxrkytd.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/grsxkdubn.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.zdbjq.cn/Article/details/gzlqetspa.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.zdbjq.cn/Article/details/gltcjvivs.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.zdbjq.cn/Article/details/gqfsbblyz.sHtML

[R61] 磁盘占用
来源：http://m.share.zdbjq.cn/Article/details/gbtrjhzod.sHtML

df -h;  du -sh *
来源：http://www.share.hesvh.cn/Article/details/gigcoyunn.sHtML

[R62] 找最占空间的文件
来源：http://wap.fehbvm.com/Article/details/ggzkzbwak.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.hesvh.cn/Article/details/grjbybdub.sHtML

[R63] 内存与进程
来源：http://wap.fehbvm.com/Article/details/geljiuoju.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.hesvh.cn/Article/details/gtkwqtbre.sHtML

[R64] 结束进程
来源：http://www.share.hesvh.cn/Article/details/ggkgkhuhl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fehbvm.com/Article/details/gbyvuvkod.sHtML

[R65] 查看端口占用
来源：http://3g.fehbvm.com/Article/details/gwuuerzho.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.zdbjq.cn/Article/details/gmmrmqzhy.sHtML

[R66] 定时任务
来源：http://mobile.zdbjq.cn/Article/details/gvimstiyi.sHtML

crontab -e;  crontab -l
来源：http://wap.zdbjq.cn/Article/details/gvavnphkw.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.hesvh.cn/Article/details/gqccshofp.sHtML

openssl rand -hex 16
来源：http://www.share.fehbvm.com/Article/details/gmjvtjyyq.sHtML

[R68] 计算文件校验值
来源：http://www.blog.hesvh.cn/Article/details/gxfwpwhuo.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.hesvh.cn/Article/details/gricoknfs.sHtML

[R69] 生成随机密码
来源：http://www.share.fehbvm.com/Article/details/goegvhjct.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.hesvh.cn/Article/details/gcofirrhg.sHtML

[R70] 时间戳与互转
来源：http://blog.zdbjq.cn/Article/details/gcsubmgdi.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.zdbjq.cn/Article/details/gndjgpbhw.sHtML

[R71] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/gqcpnafok.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.zdbjq.cn/Article/details/gvxdrfviv.sHtML

[R72] 等待端口就绪
来源：http://baike.hesvh.cn/Article/details/gjnokolrj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gdmfmzoga.sHtML

[R73] 分割大日志
来源：http://www.share.fehbvm.com/Article/details/gkagdbrqo.sHtML

split -l 1000 big.log part_
来源：http://wap.zdbjq.cn/Article/details/gzqhixuil.sHtML

[R74] 批量重命名
来源：http://3g.fehbvm.com/Article/details/gnjygnmie.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.zdbjq.cn/Article/details/glgulgvjx.sHtML

[R75] 导出环境变量
来源：http://www.blog.fehbvm.com/Article/details/gaddoxoqk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.zdbjq.cn/Article/details/gfqthkuzz.sHtML

[R76] 使用临时文件
来源：http://baike.zdbjq.cn/Article/details/gdvyvgesb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gquffgyyr.sHtML

[R77] 读取用户输入
来源：http://wap.fehbvm.com/Article/details/glgydqwla.sHtML

read -rp "请输入: " ans
来源：http://3g.fehbvm.com/Article/details/gqkhpruvj.sHtML

[R78] 交互式菜单
来源：http://m.share.zdbjq.cn/Article/details/ghdfcyupu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.hesvh.cn/Article/details/gwthpphcd.sHtML

[R79] 解析命令行选项
来源：http://blog.fehbvm.com/Article/details/gzbgqnpnu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.zdbjq.cn/Article/details/geofqhudx.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fehbvm.com/Article/details/gybgekevk.sHtML

time ./run.sh
来源：http://baike.zdbjq.cn/Article/details/gzarpbndp.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gyecwgayw.sHtML

S. C / C++ 专题
来源：http://mobile.zdbjq.cn/Article/details/ghxwjmqej.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ghwijbxsm.sHtML

[S01] C：Hello World
来源：http://www.blog.hesvh.cn/Article/details/groizlbpn.sHtML

#include <stdio.h>
来源：http://baike.hesvh.cn/Article/details/gvsoammyk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.hesvh.cn/Article/details/gkhrwwdny.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fehbvm.com/Article/details/gutickymv.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.zdbjq.cn/Article/details/gwokydyle.sHtML

[S03] C：读入整数
来源：http://www.share.zdbjq.cn/Article/details/gwbenjvim.sHtML

int x; scanf("%d", &x);
来源：http://3g.hesvh.cn/Article/details/goulmwtkk.sHtML

[S04] C：字符串复制
来源：http://read.share.zdbjq.cn/Article/details/gmxumeruw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gkprlorbm.sHtML

[S05] C：字符串长度
来源：http://blog.hesvh.cn/Article/details/gpcqwbdvg.sHtML

strlen(s)
来源：http://wap.fehbvm.com/Article/details/grdhckluz.sHtML

[S06] C：字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/guvujkgym.sHtML

strcmp(a, b) == 0
来源：http://read.share.fehbvm.com/Article/details/gjnmevqwf.sHtML

[S07] C：数组遍历求和
来源：http://baike.hesvh.cn/Article/details/gcutvikps.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.hesvh.cn/Article/details/gjcvhvdzn.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fehbvm.com/Article/details/gkirhclqg.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fehbvm.com/Article/details/gyqshjcbk.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.hesvh.cn/Article/details/gluooekbj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.zdbjq.cn/Article/details/gvvreiqud.sHtML

[S10] C：指针与解引用
来源：http://wap.fehbvm.com/Article/details/gsxsrajxt.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.hesvh.cn/Article/details/gvtytxple.sHtML

[S11] C：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gdpkukrdl.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fehbvm.com/Article/details/gzrswwlsc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.zdbjq.cn/Article/details/gnkyzxggr.sHtML

fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/gaawfkitf.sHtML

[S12] C：写文件
来源：http://m.share.hesvh.cn/Article/details/gjirpwwcl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fehbvm.com/Article/details/gtbbwzrgl.sHtML

[S13] C：宏定义
来源：http://www.blog.fehbvm.com/Article/details/gcyplafej.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fehbvm.com/Article/details/glgtatzgd.sHtML

[S14] C：枚举
来源：http://www.blog.zdbjq.cn/Article/details/ghdvbpfav.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fehbvm.com/Article/details/gcfsnbhnm.sHtML

[S15] C：类型转换
来源：http://wap.hesvh.cn/Article/details/gqfhjfhyy.sHtML

(double) a / b
来源：http://baike.fehbvm.com/Article/details/gkmqjzifo.sHtML

[S16] C：位操作置位
来源：http://blog.hesvh.cn/Article/details/gxvehwpnj.sHtML


<!-- 参考信息 -->