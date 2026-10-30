代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/grbhjnxvr.sHtML

[Q50] 批量更新
来源：http://mobile.fanxiaobao.xyz/Article/details/gdtiasqfa.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.fanxiaobao.xyz/Article/details/gkkkocqva.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gopltlmhl.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbioqlgqe.sHtML

[Q52] 删除指定行
来源：http://read.share.fanxiaobao.xyz/Article/details/ghummafxz.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzkbgtto.sHtML

[Q53] 按条件删除
来源：http://m.share.fanxiaobao.xyz/Article/details/guanwbnbp.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggpbsqxkx.sHtML

[Q54] 清空表
来源：http://blog.fanxiaobao.xyz/Article/details/gjdpbwafq.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fanxiaobao.xyz/Article/details/gqqffviak.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fanxiaobao.xyz/Article/details/geileibxj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtabbeeae.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fanxiaobao.xyz/Article/details/gumrjakfu.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guwouebkh.sHtML

[Q57] 行号
来源：http://www.share.fanxiaobao.xyz/Article/details/gtftrrnnr.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzhlcoetd.sHtML

[Q58] 累计求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gouzdljax.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gkwbcskgz.sHtML

[Q59] 分组内累计
来源：http://wap.fanxiaobao.xyz/Article/details/gnmzjjygu.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghdjxyqkk.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fanxiaobao.xyz/Article/details/gzvsyneql.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fanxiaobao.xyz/Article/details/gnkkmqxkt.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gjovspioh.sHtML

[Q61] 移动平均
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjardptkn.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gtbrkcqwf.sHtML

[Q62] 分组占比
来源：http://3g.fanxiaobao.xyz/Article/details/gzkdpyyfa.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmhoaldfo.sHtML

[Q63] 开启事务
来源：http://wap.fanxiaobao.xyz/Article/details/gdtfrrowl.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fanxiaobao.xyz/Article/details/gnrhcpsvz.sHtML

[Q64] 提交事务
来源：http://mobile.fanxiaobao.xyz/Article/details/grqptxfjl.sHtML

COMMIT;
来源：http://wap.fanxiaobao.xyz/Article/details/gisgldvyb.sHtML

[Q65] 回滚事务
来源：http://blog.fanxiaobao.xyz/Article/details/gkhqebtwv.sHtML

ROLLBACK;
来源：http://m.share.fanxiaobao.xyz/Article/details/gicmelfoo.sHtML

[Q66] 行锁查询
来源：http://blog.fanxiaobao.xyz/Article/details/gimxivdjq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fanxiaobao.xyz/Article/details/gaalpcsln.sHtML

[Q67] 设置隔离级别
来源：http://baike.fanxiaobao.xyz/Article/details/gmimhfzld.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gewvcxuri.sHtML

[Q68] 保存点
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwjbnsgrl.sHtML

SAVEPOINT sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/gldirsqfw.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gygsvbbau.sHtML

[Q69] 查看执行计划
来源：http://m.share.fanxiaobao.xyz/Article/details/gbwivvdqi.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fanxiaobao.xyz/Article/details/gquvtklfz.sHtML

[Q70] 更新统计信息
来源：http://3g.fanxiaobao.xyz/Article/details/gsxkucukz.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpuxbhjpx.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fanxiaobao.xyz/Article/details/genrjjrmu.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.fanxiaobao.xyz/Article/details/gevkmqduw.sHtML

[Q72] 查看索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gilfmtnki.sHtML

SHOW INDEX FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gmlhpicyk.sHtML

[Q73] 查看表状态
来源：http://3g.fanxiaobao.xyz/Article/details/ggxxwopep.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/gosrgmnco.sHtML

[Q74] 强制使用索引
来源：http://mobile.fanxiaobao.xyz/Article/details/grsplfesl.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fanxiaobao.xyz/Article/details/gzugqicki.sHtML

[Q75] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gikztrtth.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/ghuqkgstc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fanxiaobao.xyz/Article/details/gswsgcvbv.sHtML

[Q76] 按天统计
来源：http://m.share.fanxiaobao.xyz/Article/details/gwoifmsur.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fanxiaobao.xyz/Article/details/gcvxnznpr.sHtML

[Q77] 时间加减
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtvlnvfbk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcnushgpi.sHtML

[Q78] 当前时间
来源：http://3g.fanxiaobao.xyz/Article/details/gicbtcdac.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fanxiaobao.xyz/Article/details/gowcqbntx.sHtML

[Q79] 字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/gggddjgrt.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdavpeuxt.sHtML

[Q80] 字符串截取
来源：http://3g.fanxiaobao.xyz/Article/details/gwstadnts.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gibxuqnzh.sHtML

[Q81] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/glocndkem.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkmhkzrdy.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gahlgvrtp.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdivzslup.sHtML

[Q83] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/geedojjir.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnvrmvjys.sHtML

[Q84] 去除首尾空格
来源：http://3g.fanxiaobao.xyz/Article/details/gnaewlcpe.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gunsbkiye.sHtML

[Q85] 数值取整
来源：http://read.share.fanxiaobao.xyz/Article/details/gcejbvuta.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fanxiaobao.xyz/Article/details/gpojblixl.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fanxiaobao.xyz/Article/details/gtoqptjbf.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fanxiaobao.xyz/Article/details/gppdhzbke.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gvotkqvqx.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghfjzzlbz.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fanxiaobao.xyz/Article/details/gwbgjoaso.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fanxiaobao.xyz/Article/details/gfwzgpwcg.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gtifpwmff.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gjdefzmtj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/geordulit.sHtML

[Q90] 生成序号列
来源：http://3g.fanxiaobao.xyz/Article/details/ggzkigawa.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fanxiaobao.xyz/Article/details/glutvoxzb.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozduasay.sHtML

R. Bash 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvrzixfe.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/ghonclbtf.sHtML

[R01] shebang 与严格模式
来源：http://wap.fanxiaobao.xyz/Article/details/gefcndhab.sHtML

#!/usr/bin/env bash
来源：http://mobile.fanxiaobao.xyz/Article/details/gymlveeaa.sHtML

set -euo pipefail
来源：http://blog.fanxiaobao.xyz/Article/details/gfmtcfyqk.sHtML

[R02] 变量赋值与使用
来源：http://baike.fanxiaobao.xyz/Article/details/gwkslkicv.sHtML

name="Tom"; echo "$name"
来源：http://baike.fanxiaobao.xyz/Article/details/gvljxonwt.sHtML

[R03] 只读变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyualunib.sHtML

readonly PI=3.14
来源：http://www.blog.fanxiaobao.xyz/Article/details/goawhiflh.sHtML

[R04] 位置参数
来源：http://blog.fanxiaobao.xyz/Article/details/gqgqwgifi.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fanxiaobao.xyz/Article/details/gvyfcxlkf.sHtML

[R05] 参数默认值
来源：http://3g.fanxiaobao.xyz/Article/details/gvchlrohc.sHtML

name="${1:-default}"
来源：http://3g.fanxiaobao.xyz/Article/details/guoyxjrij.sHtML

[R06] 判断命令是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/grbxvzpgm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gotgojtpx.sHtML

[R07] if 判断文件
来源：http://read.share.fanxiaobao.xyz/Article/details/goronntcj.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gkbarmoxw.sHtML

[R08] 数值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gjwhvnydo.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmlpkrsjd.sHtML

[R09] 字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gfrhfuzls.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gavjudxik.sHtML

[R10] 正则匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/glinrfhlo.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/grbwjapnk.sHtML

[R11] case 多分支
来源：http://mobile.fanxiaobao.xyz/Article/details/gyiafiyva.sHtML

case "$1" in
来源：http://wap.fanxiaobao.xyz/Article/details/gkrpuxqlz.sHtML

start) echo "启动" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbpvzqymj.sHtML

stop)  echo "停止" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/guggihttw.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gztousnne.sHtML

esac
来源：http://mobile.fanxiaobao.xyz/Article/details/gtbadxsdf.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvevlsghn.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fanxiaobao.xyz/Article/details/grywwzkoo.sHtML

[R13] for 计数循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gisbcrbun.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gptqpaboa.sHtML

[R14] C 风格 for
来源：http://baike.fanxiaobao.xyz/Article/details/guxxgydmr.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/ggdgrrjor.sHtML

[R15] while 逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gftbrxjzp.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gpzxkogev.sHtML

[R16] until 等待条件
来源：http://blog.fanxiaobao.xyz/Article/details/glwgsheyu.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gymwzxtdr.sHtML

[R17] 数组定义与取值
来源：http://3g.fanxiaobao.xyz/Article/details/glshashnk.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gmyslbhds.sHtML

[R18] 遍历数组
来源：http://baike.fanxiaobao.xyz/Article/details/gpwbabdhm.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gkpeuxxyl.sHtML

[R19] 数组长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gvxazxefs.sHtML

echo "${#arr[@]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gjjtgpemf.sHtML

[R20] 关联数组（字典）
来源：http://3g.fanxiaobao.xyz/Article/details/gqvbuloqp.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gexwdiiux.sHtML

[R21] 字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gmyhacchn.sHtML

echo "${#s}"
来源：http://wap.fanxiaobao.xyz/Article/details/geranzecm.sHtML

[R22] 截取子串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxasfrvts.sHtML

echo "${s:0:5}"
来源：http://wap.fanxiaobao.xyz/Article/details/gqseprpnd.sHtML

[R23] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdwaakqhe.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fanxiaobao.xyz/Article/details/griajdvfo.sHtML

[R24] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/gfpcviudy.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fanxiaobao.xyz/Article/details/gboqwzicx.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fanxiaobao.xyz/Article/details/gdjpuegyd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gprzqulqw.sHtML

[R26] 命令替换
来源：http://wap.fanxiaobao.xyz/Article/details/goezuvcck.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fanxiaobao.xyz/Article/details/glngorfww.sHtML

[R27] 算术展开
来源：http://blog.fanxiaobao.xyz/Article/details/gikajluml.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glyuycfjn.sHtML

[R28] 浮点运算
来源：http://mobile.fanxiaobao.xyz/Article/details/gidsgepcj.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fanxiaobao.xyz/Article/details/gkhlcupbn.sHtML

[R29] 定义函数
来源：http://baike.fanxiaobao.xyz/Article/details/gvhjtxzhf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glcyahdea.sHtML

[R30] 函数返回状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gdoaecnkj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fanxiaobao.xyz/Article/details/guahtlimw.sHtML

[R31] 局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gikfsfurp.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/goqsuozdn.sHtML

[R32] 参数个数校验
来源：http://baike.fanxiaobao.xyz/Article/details/gkdnbaikq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gzgurwrxc.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gboafphmx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fanxiaobao.xyz/Article/details/gbewslkws.sHtML

[R34] 退出时清理
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjvsigmj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gjudraxbh.sHtML

[R35] 后台执行并等待
来源：http://www.share.fanxiaobao.xyz/Article/details/gqhuqrgmn.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fanxiaobao.xyz/Article/details/gxdjiugib.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gpfgrccok.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fanxiaobao.xyz/Article/details/glwpfhory.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gcydxyzgj.sHtML

files=$(ls -1)
来源：http://baike.fanxiaobao.xyz/Article/details/guschfels.sHtML

[R38] 管道串联
来源：http://www.share.fanxiaobao.xyz/Article/details/gorgipgat.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwqlpmust.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fanxiaobao.xyz/Article/details/gzkpssuhp.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gakyrtaoy.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnxgaswys.sHtML

echo "log" >> out.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gfrsnialy.sHtML

[R41] 丢弃输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjikgpbk.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gvrkvpolv.sHtML

[R42] 输入重定向
来源：http://wap.fanxiaobao.xyz/Article/details/glvermkvh.sHtML

wc -l < a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gbnsxjmjk.sHtML

[R43] 按名字查找文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gmcbrjsqp.sHtML

find . -name "*.log" -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/greenythq.sHtML

[R44] 按修改时间查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gwsqegnix.sHtML

find . -mtime -7 -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/glprviqfv.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvmhssdao.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fanxiaobao.xyz/Article/details/gmdxgstqt.sHtML

[R46] 递归替换文件内容
来源：http://wap.fanxiaobao.xyz/Article/details/gkbsdnunf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fanxiaobao.xyz/Article/details/gslmaemip.sHtML

[R47] sed 单行替换
来源：http://wap.fanxiaobao.xyz/Article/details/ggkpcxwtr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gtshqeiqa.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gqqgtgsky.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gibagdzvk.sHtML

[R49] awk 带条件
来源：http://blog.fanxiaobao.xyz/Article/details/guzefjxzn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqgikodmh.sHtML

[R50] awk 求和
来源：http://read.share.fanxiaobao.xyz/Article/details/glnvxjvuw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gpvnxklxc.sHtML

[R51] 排序去重取前几
来源：http://blog.fanxiaobao.xyz/Article/details/gjttqjkjb.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fanxiaobao.xyz/Article/details/gsvqwynte.sHtML

[R52] 统计行数
来源：http://read.share.fanxiaobao.xyz/Article/details/gmqymwtco.sHtML

wc -l a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gzrzplvwe.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghlzdzqgl.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gdmjpokly.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gspxrmrng.sHtML

diff a.txt b.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gitcanbuj.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/gqxktndjv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fanxiaobao.xyz/Article/details/gwhrttmgt.sHtML

[R56] 远程拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gwavmyxdv.sHtML

scp file user@host:/path/
来源：http://3g.fanxiaobao.xyz/Article/details/gdyywired.sHtML

[R57] 远程执行命令
来源：http://www.blog.fanxiaobao.xyz/Article/details/gygmtqsfm.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmvwiymg.sHtML

[R58] 下载文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gbkhraymm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fanxiaobao.xyz/Article/details/gmrtcaqvc.sHtML

[R59] 发 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/gukykbehc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fanxiaobao.xyz/Article/details/gjmysopkt.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/ggmxodgqv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fanxiaobao.xyz/Article/details/gsadshdtp.sHtML

[R61] 磁盘占用
来源：http://wap.fanxiaobao.xyz/Article/details/gpkamejqd.sHtML

df -h;  du -sh *
来源：http://mobile.fanxiaobao.xyz/Article/details/gagklhuqw.sHtML

[R62] 找最占空间的文件
来源：http://3g.fanxiaobao.xyz/Article/details/gzpcrvfro.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fanxiaobao.xyz/Article/details/ghnodzotw.sHtML

[R63] 内存与进程
来源：http://3g.fanxiaobao.xyz/Article/details/gdztsuwft.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fanxiaobao.xyz/Article/details/gzvxugjxa.sHtML

[R64] 结束进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gppuxcsko.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fanxiaobao.xyz/Article/details/gliptzubp.sHtML

[R65] 查看端口占用
来源：http://wap.fanxiaobao.xyz/Article/details/giuznejon.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/ghbgpkzsj.sHtML

[R66] 定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gamdhqvjr.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggtujvpru.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpxuuwdee.sHtML

openssl rand -hex 16
来源：http://blog.fanxiaobao.xyz/Article/details/gbkcvxkiy.sHtML

[R68] 计算文件校验值
来源：http://3g.fanxiaobao.xyz/Article/details/giaqgpitu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gssfajifz.sHtML

[R69] 生成随机密码
来源：http://www.blog.fanxiaobao.xyz/Article/details/goctlqvgd.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxdkpzltx.sHtML

[R70] 时间戳与互转
来源：http://3g.fanxiaobao.xyz/Article/details/gtsugntnc.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpjxnmsld.sHtML

[R71] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gineqklxy.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fanxiaobao.xyz/Article/details/goaazlvhe.sHtML

[R72] 等待端口就绪
来源：http://mobile.fanxiaobao.xyz/Article/details/ggioluqef.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gsdqhwggg.sHtML

[R73] 分割大日志
来源：http://blog.fanxiaobao.xyz/Article/details/gelvoyvou.sHtML

split -l 1000 big.log part_
来源：http://m.share.fanxiaobao.xyz/Article/details/gcbrcqysp.sHtML

[R74] 批量重命名
来源：http://baike.fanxiaobao.xyz/Article/details/ghammlncp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gvgwvxnoa.sHtML

[R75] 导出环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/glawahbyi.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fanxiaobao.xyz/Article/details/guplfrnge.sHtML

[R76] 使用临时文件
来源：http://3g.fanxiaobao.xyz/Article/details/gevxojkyd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsnqckftl.sHtML

[R77] 读取用户输入
来源：http://mobile.fanxiaobao.xyz/Article/details/gasrhqhhl.sHtML

read -rp "请输入: " ans
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmdmxzkd.sHtML

[R78] 交互式菜单
来源：http://blog.fanxiaobao.xyz/Article/details/glqheydjg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gclgjfiep.sHtML

[R79] 解析命令行选项
来源：http://wap.fanxiaobao.xyz/Article/details/gnkivcerb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gslvujrwq.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fanxiaobao.xyz/Article/details/gauuwolzy.sHtML

time ./run.sh
来源：http://3g.fanxiaobao.xyz/Article/details/gvhegbryj.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gqtpreggf.sHtML

S. C / C++ 专题
来源：http://baike.fanxiaobao.xyz/Article/details/glpajwkyq.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/guekrhdas.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gmofgjnet.sHtML

#include <stdio.h>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdcjmeeux.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gapkvsamd.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fanxiaobao.xyz/Article/details/gtaekgczy.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gnrdcxfjl.sHtML

[S03] C：读入整数
来源：http://m.share.fanxiaobao.xyz/Article/details/gdnbtxfek.sHtML

int x; scanf("%d", &x);
来源：http://blog.fanxiaobao.xyz/Article/details/glszyebrd.sHtML

[S04] C：字符串复制
来源：http://3g.fanxiaobao.xyz/Article/details/ggszwtajk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fanxiaobao.xyz/Article/details/ggbpxfffd.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrwroxuh.sHtML

strlen(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpxbmsynd.sHtML

[S06] C：字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gldcgqgsm.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giwpqbstc.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fanxiaobao.xyz/Article/details/grfrhpeuf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhspezla.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fanxiaobao.xyz/Article/details/gtewyamnq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdfhsvgbb.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fanxiaobao.xyz/Article/details/gelgauleg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fanxiaobao.xyz/Article/details/gpilkmcyy.sHtML

[S10] C：指针与解引用
来源：http://3g.fanxiaobao.xyz/Article/details/gtnbqbqnv.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fanxiaobao.xyz/Article/details/gcutchuyj.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gzampyild.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/gposfqdrz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxtqftfdu.sHtML

fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbamworu.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqkgartq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwadqzjvb.sHtML

[S13] C：宏定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gkgabvjjp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fanxiaobao.xyz/Article/details/gbuszqzrx.sHtML

[S14] C：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gzjopsrtv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdzcczvax.sHtML

[S15] C：类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gusmoxfhg.sHtML

(double) a / b
来源：http://3g.fanxiaobao.xyz/Article/details/ggelqtark.sHtML

[S16] C：位操作置位
来源：http://3g.fanxiaobao.xyz/Article/details/gdjvatgfj.sHtML

x |= (1 << 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gswxrjtqk.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gdzbnfnrh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtwxfzxvd.sHtML

[S18] C：命令行参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gqgaykuyy.sHtML

int main(int argc, char **argv)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnlnsnjks.sHtML

[S19] C：快速排序
来源：http://wap.fanxiaobao.xyz/Article/details/godpzyikf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gorxgutkx.sHtML

[S20] C：二分查找
来源：http://blog.fanxiaobao.xyz/Article/details/gkegwfakj.sHtML


<!-- 参考信息 -->