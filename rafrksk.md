代发 wailian999

[Q48] CTE 公用表表达式
来源：http://mobile.fehbvm.com/Article/details/glwpmcsvp.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.hesvh.cn/Article/details/gqvujdakh.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.hesvh.cn/Article/details/gjacptzfk.sHtML

[Q49] 更新单行
来源：http://www.blog.zdbjq.cn/Article/details/gfnzofwic.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/gwqysblcb.sHtML

[Q50] 批量更新
来源：http://read.share.zdbjq.cn/Article/details/gbdatdkxa.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.zdbjq.cn/Article/details/gqmozseau.sHtML

[Q51] 用子查询更新
来源：http://3g.zdbjq.cn/Article/details/gmnfqnvql.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.fehbvm.com/Article/details/gyqoikmsn.sHtML

[Q52] 删除指定行
来源：http://m.share.fehbvm.com/Article/details/gzycwplmo.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/gpwfidhbb.sHtML

[Q53] 按条件删除
来源：http://www.blog.zdbjq.cn/Article/details/grpxakqju.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.hesvh.cn/Article/details/gfwrtawkp.sHtML

[Q54] 清空表
来源：http://www.share.fehbvm.com/Article/details/gqtqsuqof.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fehbvm.com/Article/details/gzwgrwlmt.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fehbvm.com/Article/details/gjgjojtkp.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/gehxvqoge.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.fehbvm.com/Article/details/geapjxwfp.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.hesvh.cn/Article/details/gqzkrzbrn.sHtML

[Q57] 行号
来源：http://3g.hesvh.cn/Article/details/gynwvjbax.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.hesvh.cn/Article/details/gzhemsbzo.sHtML

[Q58] 累计求和
来源：http://mobile.fehbvm.com/Article/details/gfrjfxewu.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gwqmwbzkf.sHtML

[Q59] 分组内累计
来源：http://blog.fehbvm.com/Article/details/grywtfruj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gunfpiaes.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.hesvh.cn/Article/details/gfrbkklel.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.fehbvm.com/Article/details/gfgytofaz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gzdzocxfd.sHtML

[Q61] 移动平均
来源：http://3g.hesvh.cn/Article/details/gzziffuvx.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/ghmqksbzr.sHtML

[Q62] 分组占比
来源：http://blog.fehbvm.com/Article/details/ggmpopycj.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gzmvzzwrp.sHtML

[Q63] 开启事务
来源：http://mobile.hesvh.cn/Article/details/gkxjowxuj.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fehbvm.com/Article/details/gvtjjgism.sHtML

[Q64] 提交事务
来源：http://blog.zdbjq.cn/Article/details/gwpqurtqi.sHtML

COMMIT;
来源：http://3g.zdbjq.cn/Article/details/glqqsycnf.sHtML

[Q65] 回滚事务
来源：http://read.share.fehbvm.com/Article/details/gannrvsvs.sHtML

ROLLBACK;
来源：http://read.share.hesvh.cn/Article/details/gdsdugbei.sHtML

[Q66] 行锁查询
来源：http://wap.hesvh.cn/Article/details/gnwwsquto.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.hesvh.cn/Article/details/gkbhqympm.sHtML

[Q67] 设置隔离级别
来源：http://wap.fehbvm.com/Article/details/gzvscdnin.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.zdbjq.cn/Article/details/gbdrfkxfx.sHtML

[Q68] 保存点
来源：http://www.m.share.hesvh.cn/Article/details/gleffwfbq.sHtML

SAVEPOINT sp1;
来源：http://3g.hesvh.cn/Article/details/gdoifjslh.sHtML

ROLLBACK TO sp1;
来源：http://wap.hesvh.cn/Article/details/goszgunns.sHtML

[Q69] 查看执行计划
来源：http://www.share.fehbvm.com/Article/details/gkrhzyymy.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.zdbjq.cn/Article/details/gcshgrlgq.sHtML

[Q70] 更新统计信息
来源：http://3g.fehbvm.com/Article/details/glzzmjque.sHtML

ANALYZE TABLE users;
来源：http://wap.hesvh.cn/Article/details/gunutecfc.sHtML

[Q71] 查看建表语句
来源：http://m.share.hesvh.cn/Article/details/gitaigjrs.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.zdbjq.cn/Article/details/gzfywslkn.sHtML

[Q72] 查看索引
来源：http://m.share.hesvh.cn/Article/details/gwcmnzhon.sHtML

SHOW INDEX FROM users;
来源：http://wap.hesvh.cn/Article/details/gcewqbcqc.sHtML

[Q73] 查看表状态
来源：http://read.share.zdbjq.cn/Article/details/gmluekjux.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fehbvm.com/Article/details/gazkkjqag.sHtML

[Q74] 强制使用索引
来源：http://www.share.fehbvm.com/Article/details/girzbjyhv.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fehbvm.com/Article/details/gebksqnep.sHtML

[Q75] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gfqgnpsyv.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fehbvm.com/Article/details/gkugcvicq.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fehbvm.com/Article/details/gjxkbhnpb.sHtML

[Q76] 按天统计
来源：http://www.share.fehbvm.com/Article/details/gluzvdvtc.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.zdbjq.cn/Article/details/gktvcwzpy.sHtML

[Q77] 时间加减
来源：http://m.share.fehbvm.com/Article/details/geyekvnpe.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fehbvm.com/Article/details/gspgjsygs.sHtML

[Q78] 当前时间
来源：http://m.share.hesvh.cn/Article/details/gcybtvhvq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.zdbjq.cn/Article/details/gvvgihdnw.sHtML

[Q79] 字符串拼接
来源：http://read.share.hesvh.cn/Article/details/gkbmbiqzz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.zdbjq.cn/Article/details/gydgkhlbf.sHtML

[Q80] 字符串截取
来源：http://wap.fehbvm.com/Article/details/grsyjwjtz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gajjnpsxt.sHtML

[Q81] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/gghsffmoa.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.fehbvm.com/Article/details/gdtxobvpo.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fehbvm.com/Article/details/gcojqhuam.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gwavpjzxb.sHtML

[Q83] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/getgvtyej.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gxjsertxc.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fehbvm.com/Article/details/gewezlcou.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gtazkxbtg.sHtML

[Q85] 数值取整
来源：http://baike.hesvh.cn/Article/details/giyovhvjj.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.hesvh.cn/Article/details/gywohmojg.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fehbvm.com/Article/details/gjikawqky.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.hesvh.cn/Article/details/gcjipnslg.sHtML

[Q87] JSON 字段做条件
来源：http://blog.zdbjq.cn/Article/details/gjotyzrmg.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.hesvh.cn/Article/details/gghjhtzbi.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.hesvh.cn/Article/details/gndnzvwcs.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.hesvh.cn/Article/details/gxknuqmkv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gwvovcobb.sHtML

[Q89] 判断表是否存在
来源：http://blog.zdbjq.cn/Article/details/gqdcpoqdm.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fehbvm.com/Article/details/ghmcvmvpp.sHtML

[Q90] 生成序号列
来源：http://read.share.zdbjq.cn/Article/details/gnziwkcbx.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.zdbjq.cn/Article/details/gkvipevrp.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ggpygwhqy.sHtML

R. Bash 专题
来源：http://baike.fehbvm.com/Article/details/gkeabvcpy.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gocfrpzcm.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fehbvm.com/Article/details/ggduuhsnd.sHtML

#!/usr/bin/env bash
来源：http://m.share.fehbvm.com/Article/details/gqgzfqfxn.sHtML

set -euo pipefail
来源：http://wap.fehbvm.com/Article/details/gqnadlrqd.sHtML

[R02] 变量赋值与使用
来源：http://baike.fehbvm.com/Article/details/ggmmmqwrf.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fehbvm.com/Article/details/gsqvfdgan.sHtML

[R03] 只读变量
来源：http://m.share.hesvh.cn/Article/details/gymaspapj.sHtML

readonly PI=3.14
来源：http://baike.zdbjq.cn/Article/details/gcjudshbq.sHtML

[R04] 位置参数
来源：http://m.share.hesvh.cn/Article/details/gctkcphuk.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fehbvm.com/Article/details/gygvnfkcr.sHtML

[R05] 参数默认值
来源：http://baike.hesvh.cn/Article/details/gwvmnplyy.sHtML

name="${1:-default}"
来源：http://3g.hesvh.cn/Article/details/gczvsujdi.sHtML

[R06] 判断命令是否存在
来源：http://mobile.zdbjq.cn/Article/details/grubtrgkr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.zdbjq.cn/Article/details/gnyuxxpsx.sHtML

[R07] if 判断文件
来源：http://blog.hesvh.cn/Article/details/ghepfdwxr.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.hesvh.cn/Article/details/gsvxbibjs.sHtML

[R08] 数值比较
来源：http://blog.fehbvm.com/Article/details/gzagvoxad.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.zdbjq.cn/Article/details/gcuyfwidw.sHtML

[R09] 字符串比较
来源：http://mobile.zdbjq.cn/Article/details/ghpnmbqbb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.hesvh.cn/Article/details/gfguityki.sHtML

[R10] 正则匹配
来源：http://m.share.hesvh.cn/Article/details/gknqfgufh.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fehbvm.com/Article/details/gdampshod.sHtML

[R11] case 多分支
来源：http://m.share.fehbvm.com/Article/details/gxtyocswm.sHtML

case "$1" in
来源：http://mobile.hesvh.cn/Article/details/gcpmzccii.sHtML

start) echo "启动" ;;
来源：http://blog.fehbvm.com/Article/details/gwpusvteh.sHtML

stop)  echo "停止" ;;
来源：http://wap.fehbvm.com/Article/details/gubamzrza.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.hesvh.cn/Article/details/gqruzptct.sHtML

esac
来源：http://3g.hesvh.cn/Article/details/gknrbzfyk.sHtML

[R12] for 遍历文件
来源：http://www.share.zdbjq.cn/Article/details/gwtmnivac.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fehbvm.com/Article/details/gvsgkvtea.sHtML

[R13] for 计数循环
来源：http://m.share.fehbvm.com/Article/details/gqfvvsgek.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/goveaanue.sHtML

[R14] C 风格 for
来源：http://3g.hesvh.cn/Article/details/ghioakukh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.hesvh.cn/Article/details/gsftazivr.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gvedmagww.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.zdbjq.cn/Article/details/gqdapyeyx.sHtML

[R16] until 等待条件
来源：http://read.share.zdbjq.cn/Article/details/gttsmaveg.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/glsdrultk.sHtML

[R17] 数组定义与取值
来源：http://wap.zdbjq.cn/Article/details/gkfvgvrao.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fehbvm.com/Article/details/grsgjzaea.sHtML

[R18] 遍历数组
来源：http://read.share.hesvh.cn/Article/details/gzyvmhkaf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.hesvh.cn/Article/details/gcepjxnhl.sHtML

[R19] 数组长度
来源：http://m.share.hesvh.cn/Article/details/guderdmsq.sHtML

echo "${#arr[@]}"
来源：http://baike.zdbjq.cn/Article/details/gpljnqcfa.sHtML

[R20] 关联数组（字典）
来源：http://3g.fehbvm.com/Article/details/gdnzmltjx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fehbvm.com/Article/details/glxxkkvoz.sHtML

[R21] 字符串长度
来源：http://read.share.hesvh.cn/Article/details/gnsdpdwbq.sHtML

echo "${#s}"
来源：http://baike.zdbjq.cn/Article/details/guksgatag.sHtML

[R22] 截取子串
来源：http://m.share.fehbvm.com/Article/details/gjpyiewyz.sHtML

echo "${s:0:5}"
来源：http://baike.hesvh.cn/Article/details/glishjoqh.sHtML

[R23] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/gbwyeojau.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.zdbjq.cn/Article/details/gqxdfiovg.sHtML

[R24] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/gepjukyyg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fehbvm.com/Article/details/gcsypksjw.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.zdbjq.cn/Article/details/gidxrsimg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fehbvm.com/Article/details/gfiellism.sHtML

[R26] 命令替换
来源：http://3g.hesvh.cn/Article/details/gowgarmsg.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.hesvh.cn/Article/details/gqbkfltho.sHtML

[R27] 算术展开
来源：http://3g.fehbvm.com/Article/details/gjysfycoh.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fehbvm.com/Article/details/gbkhpuztu.sHtML

[R28] 浮点运算
来源：http://m.share.zdbjq.cn/Article/details/gcywojpsj.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.zdbjq.cn/Article/details/gaerkulax.sHtML

[R29] 定义函数
来源：http://read.share.hesvh.cn/Article/details/gfxzpbexb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fehbvm.com/Article/details/gtiualfmw.sHtML

[R30] 函数返回状态码
来源：http://baike.zdbjq.cn/Article/details/gffexedkw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fehbvm.com/Article/details/gijzwqhhv.sHtML

[R31] 局部变量
来源：http://blog.fehbvm.com/Article/details/grbpmuvfl.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.zdbjq.cn/Article/details/gxycdeodi.sHtML

[R32] 参数个数校验
来源：http://3g.zdbjq.cn/Article/details/gfgyglhej.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/ghpfvwmge.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fehbvm.com/Article/details/gqiqagyjv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.zdbjq.cn/Article/details/gsxaxopmg.sHtML

[R34] 退出时清理
来源：http://baike.hesvh.cn/Article/details/gtzbwnzmj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/glytxdkbu.sHtML

[R35] 后台执行并等待
来源：http://blog.zdbjq.cn/Article/details/gcsxzwezf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.hesvh.cn/Article/details/gdeqtyplo.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fehbvm.com/Article/details/gmapfbkla.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.hesvh.cn/Article/details/gapjmqynz.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fehbvm.com/Article/details/gwppntpsi.sHtML

files=$(ls -1)
来源：http://www.m.share.zdbjq.cn/Article/details/gkfpqbsav.sHtML

[R38] 管道串联
来源：http://read.share.hesvh.cn/Article/details/grrmgqcsr.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.zdbjq.cn/Article/details/gwszdcygl.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fehbvm.com/Article/details/gflljejed.sHtML

cmd > out.log 2>&1
来源：http://read.share.zdbjq.cn/Article/details/glktjwkub.sHtML

[R40] 追加写日志
来源：http://www.share.zdbjq.cn/Article/details/gbktarmiu.sHtML

echo "log" >> out.log
来源：http://mobile.zdbjq.cn/Article/details/gfojjtqxn.sHtML

[R41] 丢弃输出
来源：http://3g.hesvh.cn/Article/details/gzzueftqu.sHtML

cmd >/dev/null 2>&1
来源：http://wap.zdbjq.cn/Article/details/gddpnnoos.sHtML

[R42] 输入重定向
来源：http://read.share.zdbjq.cn/Article/details/gtutrfgbt.sHtML

wc -l < a.txt
来源：http://wap.zdbjq.cn/Article/details/giukvylen.sHtML

[R43] 按名字查找文件
来源：http://www.blog.hesvh.cn/Article/details/glrsfubym.sHtML

find . -name "*.log" -type f
来源：http://m.share.fehbvm.com/Article/details/gcxynmyyo.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fehbvm.com/Article/details/gbobqbfqf.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.zdbjq.cn/Article/details/gpmmfydyj.sHtML

[R45] 批量删除
来源：http://www.blog.zdbjq.cn/Article/details/ggmuffdyp.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fehbvm.com/Article/details/gasnzomji.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fehbvm.com/Article/details/gigenxmvt.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.hesvh.cn/Article/details/gsdckocmz.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fehbvm.com/Article/details/gkgtedkzu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fehbvm.com/Article/details/gafacujyd.sHtML

[R48] awk 取指定列
来源：http://baike.fehbvm.com/Article/details/gqeyearpd.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fehbvm.com/Article/details/gwduzmgkt.sHtML

[R49] awk 带条件
来源：http://blog.fehbvm.com/Article/details/grxvggkpb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.hesvh.cn/Article/details/gewenmhpp.sHtML

[R50] awk 求和
来源：http://m.share.fehbvm.com/Article/details/gzdexwels.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.hesvh.cn/Article/details/gvhzwzdfs.sHtML

[R51] 排序去重取前几
来源：http://wap.fehbvm.com/Article/details/grdikqyhx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.zdbjq.cn/Article/details/gjyigognn.sHtML

[R52] 统计行数
来源：http://www.blog.fehbvm.com/Article/details/gqbcgmmnk.sHtML

wc -l a.txt
来源：http://m.share.zdbjq.cn/Article/details/gzepmskex.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.zdbjq.cn/Article/details/gpmcmxwyp.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fehbvm.com/Article/details/gqpdorhgh.sHtML

[R54] 比较两个文件
来源：http://www.blog.hesvh.cn/Article/details/gkapmvorj.sHtML

diff a.txt b.txt
来源：http://3g.zdbjq.cn/Article/details/ggpcpsdah.sHtML

[R55] 压缩与解压
来源：http://read.share.hesvh.cn/Article/details/gxseoajxk.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.hesvh.cn/Article/details/gfwkdfynb.sHtML

[R56] 远程拷贝
来源：http://blog.zdbjq.cn/Article/details/gwtkfmjkc.sHtML

scp file user@host:/path/
来源：http://mobile.zdbjq.cn/Article/details/gielvcmju.sHtML

[R57] 远程执行命令
来源：http://blog.hesvh.cn/Article/details/ghulywymh.sHtML

ssh user@host 'uptime'
来源：http://3g.fehbvm.com/Article/details/guzbxnoxd.sHtML

[R58] 下载文件
来源：http://read.share.hesvh.cn/Article/details/gowikhxrb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.zdbjq.cn/Article/details/gqkmlflvc.sHtML

[R59] 发 POST JSON
来源：http://m.share.zdbjq.cn/Article/details/gnxuvohzr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fehbvm.com/Article/details/guycbbiom.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/gtczpescw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.hesvh.cn/Article/details/gsfsgjuyv.sHtML

[R61] 磁盘占用
来源：http://www.blog.hesvh.cn/Article/details/gshpeqhhh.sHtML

df -h;  du -sh *
来源：http://3g.hesvh.cn/Article/details/gwkwlgarx.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.zdbjq.cn/Article/details/ghzniatxm.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.hesvh.cn/Article/details/gzcvaxcut.sHtML

[R63] 内存与进程
来源：http://www.blog.hesvh.cn/Article/details/gasnwoiip.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.zdbjq.cn/Article/details/gnqxqazzz.sHtML

[R64] 结束进程
来源：http://mobile.hesvh.cn/Article/details/gzcurfqik.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.zdbjq.cn/Article/details/glvaebksd.sHtML

[R65] 查看端口占用
来源：http://m.share.fehbvm.com/Article/details/gaynastpb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fehbvm.com/Article/details/gpzgvzbvc.sHtML

[R66] 定时任务
来源：http://mobile.zdbjq.cn/Article/details/gzsfoxwnf.sHtML

crontab -e;  crontab -l
来源：http://www.share.hesvh.cn/Article/details/gpxfkjpur.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fehbvm.com/Article/details/gyhrvedra.sHtML

openssl rand -hex 16
来源：http://www.share.zdbjq.cn/Article/details/gjktlyirn.sHtML

[R68] 计算文件校验值
来源：http://www.share.zdbjq.cn/Article/details/ggaukdnaw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.hesvh.cn/Article/details/gnfewusjn.sHtML

[R69] 生成随机密码
来源：http://www.m.share.zdbjq.cn/Article/details/gerskmpwl.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fehbvm.com/Article/details/gzxnqnmgw.sHtML

[R70] 时间戳与互转
来源：http://blog.zdbjq.cn/Article/details/gazrgggog.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fehbvm.com/Article/details/gswjvsnoh.sHtML

[R71] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gialcikkv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.zdbjq.cn/Article/details/gnthsjgyt.sHtML

[R72] 等待端口就绪
来源：http://mobile.hesvh.cn/Article/details/gkfppedbw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/gbdionvos.sHtML

[R73] 分割大日志
来源：http://www.share.fehbvm.com/Article/details/ggzyfxakn.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.zdbjq.cn/Article/details/gcnxjhlbo.sHtML

[R74] 批量重命名
来源：http://wap.hesvh.cn/Article/details/grstrnbci.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.hesvh.cn/Article/details/gjmcrnqpq.sHtML

[R75] 导出环境变量
来源：http://baike.zdbjq.cn/Article/details/gcvjmmicb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fehbvm.com/Article/details/gwnhiftow.sHtML

[R76] 使用临时文件
来源：http://baike.fehbvm.com/Article/details/gyptakiki.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gqfebfllf.sHtML

[R77] 读取用户输入
来源：http://wap.zdbjq.cn/Article/details/guroizfhz.sHtML

read -rp "请输入: " ans
来源：http://read.share.hesvh.cn/Article/details/geyjoytmz.sHtML

[R78] 交互式菜单
来源：http://baike.fehbvm.com/Article/details/ggclxafrk.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fehbvm.com/Article/details/ghugzmjpz.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.zdbjq.cn/Article/details/gnrjxotcu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fehbvm.com/Article/details/gpuuprvbi.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fehbvm.com/Article/details/gjclefelq.sHtML

time ./run.sh
来源：http://www.blog.hesvh.cn/Article/details/gzfctutcp.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gckomjygd.sHtML

S. C / C++ 专题
来源：http://read.share.hesvh.cn/Article/details/gmcepniws.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gknszrjgl.sHtML

[S01] C：Hello World
来源：http://blog.zdbjq.cn/Article/details/gpnivjpdq.sHtML

#include <stdio.h>
来源：http://wap.fehbvm.com/Article/details/gwmpkvcsq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.hesvh.cn/Article/details/ggyqnufxg.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.hesvh.cn/Article/details/galhxzgzc.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.zdbjq.cn/Article/details/grgnohryd.sHtML

[S03] C：读入整数
来源：http://www.share.fehbvm.com/Article/details/gpyficvuc.sHtML

int x; scanf("%d", &x);
来源：http://read.share.zdbjq.cn/Article/details/gdchvyewy.sHtML

[S04] C：字符串复制
来源：http://baike.hesvh.cn/Article/details/ghzfrxqrv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.hesvh.cn/Article/details/gghjrnmar.sHtML

[S05] C：字符串长度
来源：http://3g.zdbjq.cn/Article/details/gpdmfmolf.sHtML

strlen(s)
来源：http://read.share.hesvh.cn/Article/details/gnzotxmze.sHtML

[S06] C：字符串比较
来源：http://mobile.zdbjq.cn/Article/details/gqnzeldaq.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.zdbjq.cn/Article/details/ghplmqeqf.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fehbvm.com/Article/details/gcptzxdlh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.zdbjq.cn/Article/details/guqwaftuq.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.hesvh.cn/Article/details/gbathdapx.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fehbvm.com/Article/details/gqkhiwapp.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fehbvm.com/Article/details/gtaadibnk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.hesvh.cn/Article/details/godmpfbaf.sHtML

[S10] C：指针与解引用
来源：http://wap.zdbjq.cn/Article/details/gbszpnmaj.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.zdbjq.cn/Article/details/grpyqldwg.sHtML

[S11] C：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gwfdzvpro.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.hesvh.cn/Article/details/gdoldgusv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fehbvm.com/Article/details/gyiigvytw.sHtML

fclose(f);
来源：http://blog.hesvh.cn/Article/details/gearcfsij.sHtML

[S12] C：写文件
来源：http://baike.hesvh.cn/Article/details/ghwexkzjp.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/gvawfvura.sHtML

[S13] C：宏定义
来源：http://wap.zdbjq.cn/Article/details/gpkkimsvy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fehbvm.com/Article/details/ggxqewqxe.sHtML

[S14] C：枚举
来源：http://www.share.fehbvm.com/Article/details/goocxuxmc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fehbvm.com/Article/details/ghpxjcmzg.sHtML

[S15] C：类型转换
来源：http://blog.zdbjq.cn/Article/details/gektciglx.sHtML

(double) a / b
来源：http://blog.zdbjq.cn/Article/details/gilleqlpz.sHtML

[S16] C：位操作置位
来源：http://m.share.fehbvm.com/Article/details/gfndshxnq.sHtML

x |= (1 << 3);
来源：http://3g.zdbjq.cn/Article/details/gbfazkcvu.sHtML

[S17] C：安全拼接字符串
来源：http://3g.hesvh.cn/Article/details/ghzbzctsk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.hesvh.cn/Article/details/gcukqpqrs.sHtML

[S18] C：命令行参数
来源：http://baike.fehbvm.com/Article/details/gmogphswz.sHtML


<!-- 参考信息 -->