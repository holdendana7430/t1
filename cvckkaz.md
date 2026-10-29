代发 wailian999

[Q48] CTE 公用表表达式
来源：http://baike.hesvh.cn/Article/details/gcwdkfvso.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.fehbvm.com/Article/details/gdkrbpzim.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.zdbjq.cn/Article/details/gyounybpk.sHtML

[Q49] 更新单行
来源：http://www.m.share.hesvh.cn/Article/details/ghyirkhkj.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/gcjmolymj.sHtML

[Q50] 批量更新
来源：http://mobile.zdbjq.cn/Article/details/gqegilnkz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.zdbjq.cn/Article/details/gjajnkbzg.sHtML

[Q51] 用子查询更新
来源：http://mobile.fehbvm.com/Article/details/gvbvlmlzi.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.zdbjq.cn/Article/details/gxyquudxi.sHtML

[Q52] 删除指定行
来源：http://m.share.hesvh.cn/Article/details/gqdtmsynb.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fehbvm.com/Article/details/gtwvvcykz.sHtML

[Q53] 按条件删除
来源：http://baike.fehbvm.com/Article/details/gydeayrdw.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.hesvh.cn/Article/details/gvbyztkvx.sHtML

[Q54] 清空表
来源：http://blog.fehbvm.com/Article/details/gwzznhvnb.sHtML

TRUNCATE TABLE logs;
来源：http://blog.zdbjq.cn/Article/details/gvucjhudk.sHtML

[Q55] 排名（并列占位）
来源：http://blog.hesvh.cn/Article/details/gvudvdlgf.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.hesvh.cn/Article/details/gontgmrnw.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fehbvm.com/Article/details/gjnnijdnw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/gdyqagzud.sHtML

[Q57] 行号
来源：http://www.blog.zdbjq.cn/Article/details/guuwifbrb.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.hesvh.cn/Article/details/gymgnvjrq.sHtML

[Q58] 累计求和
来源：http://www.blog.hesvh.cn/Article/details/grpkpyyiy.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gqdhrcvce.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fehbvm.com/Article/details/gcnumozpn.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gkbhztuaf.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.hesvh.cn/Article/details/gzpwuwolq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.hesvh.cn/Article/details/gtsdbolmf.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fehbvm.com/Article/details/gnwodoijx.sHtML

[Q61] 移动平均
来源：http://baike.zdbjq.cn/Article/details/grdkobamc.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/ggpvtuuyh.sHtML

[Q62] 分组占比
来源：http://baike.fehbvm.com/Article/details/gmdsfbcxd.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/grchmzeau.sHtML

[Q63] 开启事务
来源：http://blog.fehbvm.com/Article/details/gmkrclbey.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.zdbjq.cn/Article/details/gzrcemcip.sHtML

[Q64] 提交事务
来源：http://3g.zdbjq.cn/Article/details/gajurtgcq.sHtML

COMMIT;
来源：http://3g.hesvh.cn/Article/details/gzoxnzkui.sHtML

[Q65] 回滚事务
来源：http://3g.zdbjq.cn/Article/details/gdsaboprs.sHtML

ROLLBACK;
来源：http://www.blog.hesvh.cn/Article/details/getmqihyr.sHtML

[Q66] 行锁查询
来源：http://wap.hesvh.cn/Article/details/gogmeokej.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.hesvh.cn/Article/details/gjuvdbmxq.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.hesvh.cn/Article/details/gkccbfqrf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.hesvh.cn/Article/details/gbgpwppdu.sHtML

[Q68] 保存点
来源：http://3g.fehbvm.com/Article/details/gwqjoquhd.sHtML

SAVEPOINT sp1;
来源：http://blog.hesvh.cn/Article/details/gaxjqvubh.sHtML

ROLLBACK TO sp1;
来源：http://baike.zdbjq.cn/Article/details/gfxlyonzp.sHtML

[Q69] 查看执行计划
来源：http://m.share.zdbjq.cn/Article/details/gzmsovapb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fehbvm.com/Article/details/gpurewvgs.sHtML

[Q70] 更新统计信息
来源：http://www.share.fehbvm.com/Article/details/ggqslkhem.sHtML

ANALYZE TABLE users;
来源：http://baike.hesvh.cn/Article/details/gayhgwxka.sHtML

[Q71] 查看建表语句
来源：http://www.blog.zdbjq.cn/Article/details/gvtzccxpe.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.hesvh.cn/Article/details/gwbvpwlhz.sHtML

[Q72] 查看索引
来源：http://baike.fehbvm.com/Article/details/ghsisnbmi.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gyrvulebu.sHtML

[Q73] 查看表状态
来源：http://www.blog.zdbjq.cn/Article/details/glwajjoxi.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.hesvh.cn/Article/details/goovefiww.sHtML

[Q74] 强制使用索引
来源：http://m.share.fehbvm.com/Article/details/gluwnhtks.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.hesvh.cn/Article/details/ghujdwleo.sHtML

[Q75] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/gjsxgrrsf.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gyitaqokb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.zdbjq.cn/Article/details/gpgafrqdj.sHtML

[Q76] 按天统计
来源：http://www.m.share.hesvh.cn/Article/details/gjjgtqxmo.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.hesvh.cn/Article/details/grstjplne.sHtML

[Q77] 时间加减
来源：http://baike.fehbvm.com/Article/details/gwrxtnutt.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.zdbjq.cn/Article/details/gkxemhczj.sHtML

[Q78] 当前时间
来源：http://www.blog.hesvh.cn/Article/details/gckxdvlog.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fehbvm.com/Article/details/gddkbsvoa.sHtML

[Q79] 字符串拼接
来源：http://blog.zdbjq.cn/Article/details/grjqoertf.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.hesvh.cn/Article/details/gcqvnztub.sHtML

[Q80] 字符串截取
来源：http://m.share.zdbjq.cn/Article/details/gkcfkenor.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.hesvh.cn/Article/details/grfdsdzqs.sHtML

[Q81] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/gmoljggvo.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.hesvh.cn/Article/details/gamzlkyva.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.zdbjq.cn/Article/details/ghtpiipbr.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/giyzgkkjg.sHtML

[Q83] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gwhnethcw.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/glrbniile.sHtML

[Q84] 去除首尾空格
来源：http://mobile.zdbjq.cn/Article/details/gcqdudclk.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/ggiwykjys.sHtML

[Q85] 数值取整
来源：http://baike.fehbvm.com/Article/details/gvhbsdihc.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.zdbjq.cn/Article/details/guprhzrdx.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.zdbjq.cn/Article/details/gabqntfcn.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fehbvm.com/Article/details/gichvwhwo.sHtML

[Q87] JSON 字段做条件
来源：http://blog.zdbjq.cn/Article/details/gdbpjgcok.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fehbvm.com/Article/details/gmkibdrxh.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.hesvh.cn/Article/details/guzvnwwwu.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fehbvm.com/Article/details/giukpzktj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gwatbmuuq.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fehbvm.com/Article/details/gbwkveael.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.hesvh.cn/Article/details/gldrtwnto.sHtML

[Q90] 生成序号列
来源：http://www.m.share.hesvh.cn/Article/details/ggqdetnok.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.hesvh.cn/Article/details/gvlhueemc.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/grhpxdmcn.sHtML

R. Bash 专题
来源：http://www.m.share.fehbvm.com/Article/details/gtdetqplq.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gmrrmqoiq.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fehbvm.com/Article/details/gcrzfnyhq.sHtML

#!/usr/bin/env bash
来源：http://wap.zdbjq.cn/Article/details/gcdntgiap.sHtML

set -euo pipefail
来源：http://wap.zdbjq.cn/Article/details/gnknbgodl.sHtML

[R02] 变量赋值与使用
来源：http://3g.hesvh.cn/Article/details/gligtntts.sHtML

name="Tom"; echo "$name"
来源：http://3g.zdbjq.cn/Article/details/gxaqfpzeh.sHtML

[R03] 只读变量
来源：http://www.share.hesvh.cn/Article/details/gqhmddpeb.sHtML

readonly PI=3.14
来源：http://baike.hesvh.cn/Article/details/gbpbxaiwb.sHtML

[R04] 位置参数
来源：http://www.m.share.fehbvm.com/Article/details/gxnrrkdyu.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.zdbjq.cn/Article/details/gcefnfwmy.sHtML

[R05] 参数默认值
来源：http://m.share.fehbvm.com/Article/details/gbyyhuykw.sHtML

name="${1:-default}"
来源：http://3g.fehbvm.com/Article/details/gwkrikjbx.sHtML

[R06] 判断命令是否存在
来源：http://blog.hesvh.cn/Article/details/gatgqpogl.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/gpatlkpms.sHtML

[R07] if 判断文件
来源：http://m.share.hesvh.cn/Article/details/glsczbads.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.hesvh.cn/Article/details/gkgemmvnl.sHtML

[R08] 数值比较
来源：http://read.share.zdbjq.cn/Article/details/gutfypusf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fehbvm.com/Article/details/gyzjvqalj.sHtML

[R09] 字符串比较
来源：http://read.share.zdbjq.cn/Article/details/ghaoimhod.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.zdbjq.cn/Article/details/gzbwhkdio.sHtML

[R10] 正则匹配
来源：http://read.share.fehbvm.com/Article/details/gydembqdb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.zdbjq.cn/Article/details/gpoaiqxmz.sHtML

[R11] case 多分支
来源：http://www.m.share.fehbvm.com/Article/details/gtmpvgico.sHtML

case "$1" in
来源：http://read.share.zdbjq.cn/Article/details/ghegnnyuy.sHtML

start) echo "启动" ;;
来源：http://www.blog.fehbvm.com/Article/details/gtdwpqyqq.sHtML

stop)  echo "停止" ;;
来源：http://wap.zdbjq.cn/Article/details/gjdsmohar.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fehbvm.com/Article/details/ggkpajrbg.sHtML

esac
来源：http://www.m.share.hesvh.cn/Article/details/gzqvwmuso.sHtML

[R12] for 遍历文件
来源：http://blog.hesvh.cn/Article/details/goybtgoxi.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.hesvh.cn/Article/details/gpfnkqpza.sHtML

[R13] for 计数循环
来源：http://www.m.share.zdbjq.cn/Article/details/gsccsbtqf.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/gwfcaqcmv.sHtML

[R14] C 风格 for
来源：http://wap.fehbvm.com/Article/details/gkjglsdlp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/gsbynmnvy.sHtML

[R15] while 逐行读文件
来源：http://mobile.fehbvm.com/Article/details/goarxhuke.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fehbvm.com/Article/details/getyxwhdh.sHtML

[R16] until 等待条件
来源：http://www.share.zdbjq.cn/Article/details/gopkiipsa.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/gsrdewdor.sHtML

[R17] 数组定义与取值
来源：http://mobile.zdbjq.cn/Article/details/gxmthcmub.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fehbvm.com/Article/details/gtddqcous.sHtML

[R18] 遍历数组
来源：http://read.share.zdbjq.cn/Article/details/gnfawsxvr.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fehbvm.com/Article/details/gnveqnajd.sHtML

[R19] 数组长度
来源：http://mobile.hesvh.cn/Article/details/gsraaixji.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.zdbjq.cn/Article/details/glaufnzka.sHtML

[R20] 关联数组（字典）
来源：http://read.share.zdbjq.cn/Article/details/gcqsfjoco.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fehbvm.com/Article/details/geszrmvrt.sHtML

[R21] 字符串长度
来源：http://read.share.zdbjq.cn/Article/details/gahzjuyqi.sHtML

echo "${#s}"
来源：http://m.share.zdbjq.cn/Article/details/goadctrme.sHtML

[R22] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/ggefpemhn.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fehbvm.com/Article/details/gxrdyxosk.sHtML

[R23] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/gjmcxowkw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.zdbjq.cn/Article/details/gvybxmmrw.sHtML

[R24] 大小写转换
来源：http://3g.fehbvm.com/Article/details/gmivdvofk.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fehbvm.com/Article/details/grbfxnfgv.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.hesvh.cn/Article/details/gujkdsevo.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.zdbjq.cn/Article/details/grwgospzy.sHtML

[R26] 命令替换
来源：http://read.share.fehbvm.com/Article/details/gffiaalvr.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.zdbjq.cn/Article/details/gadkmqwxn.sHtML

[R27] 算术展开
来源：http://www.share.fehbvm.com/Article/details/giddbvnwc.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fehbvm.com/Article/details/gqihhgcei.sHtML

[R28] 浮点运算
来源：http://www.m.share.fehbvm.com/Article/details/gpojnfrxt.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.zdbjq.cn/Article/details/gqxwmfwym.sHtML

[R29] 定义函数
来源：http://www.blog.zdbjq.cn/Article/details/gmqnjuuav.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.hesvh.cn/Article/details/garzvnmtb.sHtML

[R30] 函数返回状态码
来源：http://wap.fehbvm.com/Article/details/gqombpcpv.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.hesvh.cn/Article/details/gxeclhjfv.sHtML

[R31] 局部变量
来源：http://wap.zdbjq.cn/Article/details/gqvfnrsgh.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fehbvm.com/Article/details/gjcgtwhmm.sHtML

[R32] 参数个数校验
来源：http://www.share.hesvh.cn/Article/details/gzgfnfrox.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/gryeijbgz.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fehbvm.com/Article/details/gechztnlg.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.zdbjq.cn/Article/details/gsjxymtsj.sHtML

[R34] 退出时清理
来源：http://3g.fehbvm.com/Article/details/grlmradyx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/ghgbmxbeo.sHtML

[R35] 后台执行并等待
来源：http://www.share.hesvh.cn/Article/details/gmxhtowsv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fehbvm.com/Article/details/gmbrllguu.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fehbvm.com/Article/details/gnybwawqz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.zdbjq.cn/Article/details/gwwmkdaap.sHtML

[R37] 把输出赋给变量
来源：http://read.share.zdbjq.cn/Article/details/gnnlohyjg.sHtML

files=$(ls -1)
来源：http://baike.zdbjq.cn/Article/details/gyqehjyts.sHtML

[R38] 管道串联
来源：http://baike.hesvh.cn/Article/details/ghnmnqrnk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.hesvh.cn/Article/details/gjymtjavk.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fehbvm.com/Article/details/ggkxqglsx.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/gtqzshzdx.sHtML

[R40] 追加写日志
来源：http://read.share.fehbvm.com/Article/details/ggjlslimg.sHtML

echo "log" >> out.log
来源：http://mobile.hesvh.cn/Article/details/gwulqejbr.sHtML

[R41] 丢弃输出
来源：http://m.share.fehbvm.com/Article/details/gvgfahmiy.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fehbvm.com/Article/details/gqjoxkxol.sHtML

[R42] 输入重定向
来源：http://m.share.zdbjq.cn/Article/details/ggesyfbjj.sHtML

wc -l < a.txt
来源：http://read.share.hesvh.cn/Article/details/gmkhxrvhv.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fehbvm.com/Article/details/gzqblqqln.sHtML

find . -name "*.log" -type f
来源：http://read.share.fehbvm.com/Article/details/gugbsybpt.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.zdbjq.cn/Article/details/gjtaewzsm.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.zdbjq.cn/Article/details/gqyciivnq.sHtML

[R45] 批量删除
来源：http://wap.hesvh.cn/Article/details/grlambdco.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fehbvm.com/Article/details/gdvviaqsb.sHtML

[R46] 递归替换文件内容
来源：http://baike.fehbvm.com/Article/details/gmsdqewij.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.zdbjq.cn/Article/details/gtdthixee.sHtML

[R47] sed 单行替换
来源：http://www.m.share.hesvh.cn/Article/details/grdsyazzw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fehbvm.com/Article/details/ghsukflnt.sHtML

[R48] awk 取指定列
来源：http://wap.zdbjq.cn/Article/details/gkyrprnmm.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.hesvh.cn/Article/details/gprfcgizg.sHtML

[R49] awk 带条件
来源：http://m.share.fehbvm.com/Article/details/gibzodxve.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.hesvh.cn/Article/details/gyznfzjli.sHtML

[R50] awk 求和
来源：http://m.share.zdbjq.cn/Article/details/gvantyftw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.zdbjq.cn/Article/details/gaargzcww.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.zdbjq.cn/Article/details/gpclzvbft.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.hesvh.cn/Article/details/glkmmjwbk.sHtML

[R52] 统计行数
来源：http://blog.hesvh.cn/Article/details/geofyswge.sHtML

wc -l a.txt
来源：http://blog.hesvh.cn/Article/details/gqfpkwsrg.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.zdbjq.cn/Article/details/gljahtiym.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fehbvm.com/Article/details/gwnyounrh.sHtML

[R54] 比较两个文件
来源：http://m.share.hesvh.cn/Article/details/gqrnrqjak.sHtML

diff a.txt b.txt
来源：http://www.blog.fehbvm.com/Article/details/gnftlfgnf.sHtML

[R55] 压缩与解压
来源：http://3g.hesvh.cn/Article/details/gjdqkwjwx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fehbvm.com/Article/details/grulumoqr.sHtML

[R56] 远程拷贝
来源：http://read.share.zdbjq.cn/Article/details/gpymbzxoo.sHtML

scp file user@host:/path/
来源：http://www.blog.hesvh.cn/Article/details/gkutmwanb.sHtML

[R57] 远程执行命令
来源：http://www.m.share.hesvh.cn/Article/details/gevozxwhy.sHtML

ssh user@host 'uptime'
来源：http://wap.hesvh.cn/Article/details/gmwfplweo.sHtML

[R58] 下载文件
来源：http://m.share.fehbvm.com/Article/details/gpkamlnkr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.hesvh.cn/Article/details/giwictbcg.sHtML

[R59] 发 POST JSON
来源：http://baike.fehbvm.com/Article/details/gkovrtslo.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.hesvh.cn/Article/details/gxhdulibx.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/gthlikwla.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.hesvh.cn/Article/details/gzkdiciwi.sHtML

[R61] 磁盘占用
来源：http://m.share.fehbvm.com/Article/details/gftxtvmtk.sHtML

df -h;  du -sh *
来源：http://read.share.fehbvm.com/Article/details/gqwjbgbec.sHtML

[R62] 找最占空间的文件
来源：http://read.share.hesvh.cn/Article/details/gfhfslpgo.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.hesvh.cn/Article/details/gmqqfdzlh.sHtML

[R63] 内存与进程
来源：http://baike.zdbjq.cn/Article/details/giblvhcwo.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.zdbjq.cn/Article/details/gedqkuvst.sHtML

[R64] 结束进程
来源：http://mobile.zdbjq.cn/Article/details/gckdxsrpq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fehbvm.com/Article/details/ggcnuwbsf.sHtML

[R65] 查看端口占用
来源：http://m.share.hesvh.cn/Article/details/gkzhiansn.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.hesvh.cn/Article/details/ghpatocvr.sHtML

[R66] 定时任务
来源：http://www.blog.hesvh.cn/Article/details/ggmarveiv.sHtML

crontab -e;  crontab -l
来源：http://wap.hesvh.cn/Article/details/gewpnbtqi.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fehbvm.com/Article/details/gdwubezvy.sHtML

openssl rand -hex 16
来源：http://blog.fehbvm.com/Article/details/gekzujbub.sHtML

[R68] 计算文件校验值
来源：http://read.share.hesvh.cn/Article/details/gptdrwhwk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gwkfumbdv.sHtML

[R69] 生成随机密码
来源：http://baike.fehbvm.com/Article/details/ghgkeyorg.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.zdbjq.cn/Article/details/gyygujpap.sHtML

[R70] 时间戳与互转
来源：http://3g.hesvh.cn/Article/details/gapkoxhrc.sHtML

date +%s;  date -d @1700000000
来源：http://blog.zdbjq.cn/Article/details/gbbetteon.sHtML

[R71] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/grzvwfavk.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.hesvh.cn/Article/details/gvsznsltq.sHtML

[R72] 等待端口就绪
来源：http://3g.hesvh.cn/Article/details/gjrhfpxpw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gzrdmvegl.sHtML

[R73] 分割大日志
来源：http://www.blog.hesvh.cn/Article/details/gavoxsdal.sHtML

split -l 1000 big.log part_
来源：http://baike.fehbvm.com/Article/details/ghmdiblik.sHtML

[R74] 批量重命名
来源：http://mobile.zdbjq.cn/Article/details/gnoatupfw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fehbvm.com/Article/details/grhayltci.sHtML

[R75] 导出环境变量
来源：http://read.share.zdbjq.cn/Article/details/gjxdvpamv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fehbvm.com/Article/details/ghmfiggph.sHtML

[R76] 使用临时文件
来源：http://blog.hesvh.cn/Article/details/gdtbaglzr.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/gtstqxnno.sHtML

[R77] 读取用户输入
来源：http://baike.fehbvm.com/Article/details/gazgrunls.sHtML

read -rp "请输入: " ans
来源：http://m.share.fehbvm.com/Article/details/grffyhrrq.sHtML

[R78] 交互式菜单
来源：http://wap.fehbvm.com/Article/details/gwddhrxay.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.zdbjq.cn/Article/details/gagakfver.sHtML

[R79] 解析命令行选项
来源：http://m.share.hesvh.cn/Article/details/gfqmpmwsl.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.hesvh.cn/Article/details/gygjhiwlu.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fehbvm.com/Article/details/gkdxmbazz.sHtML

time ./run.sh
来源：http://mobile.hesvh.cn/Article/details/gojgqzyrm.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gllspobwt.sHtML

S. C / C++ 专题
来源：http://wap.fehbvm.com/Article/details/gbxppxevd.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/grgaodore.sHtML

[S01] C：Hello World
来源：http://baike.zdbjq.cn/Article/details/geqbibppr.sHtML

#include <stdio.h>
来源：http://blog.zdbjq.cn/Article/details/gothzorgp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.zdbjq.cn/Article/details/gdrmxsgfr.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fehbvm.com/Article/details/gkybtcmhd.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.zdbjq.cn/Article/details/gklrxzgph.sHtML

[S03] C：读入整数
来源：http://www.blog.hesvh.cn/Article/details/geeddvwgv.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fehbvm.com/Article/details/gsfdmfkwf.sHtML

[S04] C：字符串复制
来源：http://blog.fehbvm.com/Article/details/gvwbsfgin.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/giynhzkmq.sHtML

[S05] C：字符串长度
来源：http://read.share.fehbvm.com/Article/details/gooskntiv.sHtML

strlen(s)
来源：http://www.m.share.hesvh.cn/Article/details/gibcfnnuh.sHtML

[S06] C：字符串比较
来源：http://www.blog.fehbvm.com/Article/details/gfsacaonw.sHtML

strcmp(a, b) == 0
来源：http://blog.hesvh.cn/Article/details/gwqkyxsfu.sHtML

[S07] C：数组遍历求和
来源：http://3g.fehbvm.com/Article/details/gwrgwslfz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.hesvh.cn/Article/details/grfbslobu.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.hesvh.cn/Article/details/gknqjdquv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.hesvh.cn/Article/details/gpyjoxazd.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.hesvh.cn/Article/details/gtomcnbxo.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fehbvm.com/Article/details/gyvxlyqyk.sHtML

[S10] C：指针与解引用
来源：http://read.share.zdbjq.cn/Article/details/gzzeeikgv.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fehbvm.com/Article/details/gadzqjnef.sHtML

[S11] C：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/glwejsozs.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.zdbjq.cn/Article/details/gmmltenmh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.hesvh.cn/Article/details/gmvewatvr.sHtML

fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gjnsfejbk.sHtML

[S12] C：写文件
来源：http://3g.zdbjq.cn/Article/details/gvcjirqqf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.hesvh.cn/Article/details/gcogrcfew.sHtML

[S13] C：宏定义
来源：http://baike.zdbjq.cn/Article/details/gmjdttrrp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.hesvh.cn/Article/details/gqufzidpd.sHtML

[S14] C：枚举
来源：http://mobile.hesvh.cn/Article/details/ghdwtlreu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.hesvh.cn/Article/details/gbnjvcijw.sHtML

[S15] C：类型转换
来源：http://blog.zdbjq.cn/Article/details/gustpgssy.sHtML

(double) a / b
来源：http://www.share.hesvh.cn/Article/details/gjvnxpkiy.sHtML

[S16] C：位操作置位
来源：http://m.share.hesvh.cn/Article/details/gdcwlojkl.sHtML

x |= (1 << 3);
来源：http://wap.zdbjq.cn/Article/details/gphwsfbby.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gabrgkkfy.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.zdbjq.cn/Article/details/gfqgfrqze.sHtML

[S18] C：命令行参数
来源：http://www.share.hesvh.cn/Article/details/gyiutglkw.sHtML


<!-- 参考信息 -->