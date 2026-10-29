代发 wailian999

[Q48] CTE 公用表表达式
来源：http://3g.hesvh.cn/Article/details/ggllitboi.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.zdbjq.cn/Article/details/gxmnyosbj.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.zdbjq.cn/Article/details/gdfvxzkrf.sHtML

[Q49] 更新单行
来源：http://baike.fehbvm.com/Article/details/grgfwmufl.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.hesvh.cn/Article/details/gzatazvon.sHtML

[Q50] 批量更新
来源：http://www.blog.hesvh.cn/Article/details/gxuvipybz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/guhezhtyb.sHtML

[Q51] 用子查询更新
来源：http://www.share.zdbjq.cn/Article/details/gqvzxnari.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.hesvh.cn/Article/details/gdmuqmfzl.sHtML

[Q52] 删除指定行
来源：http://wap.fehbvm.com/Article/details/gwjmhbfab.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/gpuwdejiw.sHtML

[Q53] 按条件删除
来源：http://3g.fehbvm.com/Article/details/gsfmggxsu.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.hesvh.cn/Article/details/gcvqjwhlx.sHtML

[Q54] 清空表
来源：http://mobile.fehbvm.com/Article/details/gymlyodbb.sHtML

TRUNCATE TABLE logs;
来源：http://3g.zdbjq.cn/Article/details/gmxuxmsia.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.hesvh.cn/Article/details/gfrmdjrbc.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.fehbvm.com/Article/details/gpzquotcp.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.hesvh.cn/Article/details/gqkhsbhbq.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.hesvh.cn/Article/details/gswsgsuvi.sHtML

[Q57] 行号
来源：http://www.m.share.hesvh.cn/Article/details/giiibfkni.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.hesvh.cn/Article/details/gkjbgvumj.sHtML

[Q58] 累计求和
来源：http://m.share.zdbjq.cn/Article/details/gamvrajzz.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.hesvh.cn/Article/details/glfomviid.sHtML

[Q59] 分组内累计
来源：http://mobile.zdbjq.cn/Article/details/gkvqhctgb.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gatjbzgby.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fehbvm.com/Article/details/gvxqlpjxl.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.zdbjq.cn/Article/details/gmzdtkprw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/goqkcuppp.sHtML

[Q61] 移动平均
来源：http://m.share.zdbjq.cn/Article/details/gojnicxvm.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gbbfbxzov.sHtML

[Q62] 分组占比
来源：http://www.blog.hesvh.cn/Article/details/gqyyjlfgb.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gjrbiyghu.sHtML

[Q63] 开启事务
来源：http://m.share.zdbjq.cn/Article/details/gywxyshdt.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.zdbjq.cn/Article/details/gtnxxpcwa.sHtML

[Q64] 提交事务
来源：http://read.share.zdbjq.cn/Article/details/gnwozwhdi.sHtML

COMMIT;
来源：http://m.share.zdbjq.cn/Article/details/gwphazeup.sHtML

[Q65] 回滚事务
来源：http://www.blog.zdbjq.cn/Article/details/gbdviqlte.sHtML

ROLLBACK;
来源：http://www.blog.zdbjq.cn/Article/details/grgnlkost.sHtML

[Q66] 行锁查询
来源：http://www.blog.fehbvm.com/Article/details/gszzvlhwy.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.hesvh.cn/Article/details/glpuoxvab.sHtML

[Q67] 设置隔离级别
来源：http://3g.zdbjq.cn/Article/details/gancbwcbs.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fehbvm.com/Article/details/gcfzhpruh.sHtML

[Q68] 保存点
来源：http://m.share.hesvh.cn/Article/details/gylmsiurw.sHtML

SAVEPOINT sp1;
来源：http://blog.fehbvm.com/Article/details/groilhlgq.sHtML

ROLLBACK TO sp1;
来源：http://mobile.zdbjq.cn/Article/details/gnrdspque.sHtML

[Q69] 查看执行计划
来源：http://baike.zdbjq.cn/Article/details/gjauxhzvc.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fehbvm.com/Article/details/gvxqcekga.sHtML

[Q70] 更新统计信息
来源：http://mobile.hesvh.cn/Article/details/gppldyung.sHtML

ANALYZE TABLE users;
来源：http://3g.hesvh.cn/Article/details/gpibhfcwy.sHtML

[Q71] 查看建表语句
来源：http://mobile.hesvh.cn/Article/details/gzbxqklxz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fehbvm.com/Article/details/gjbydqbno.sHtML

[Q72] 查看索引
来源：http://m.share.fehbvm.com/Article/details/gcgowqkwx.sHtML

SHOW INDEX FROM users;
来源：http://blog.fehbvm.com/Article/details/gebauwfrt.sHtML

[Q73] 查看表状态
来源：http://www.share.fehbvm.com/Article/details/gsgvewaeg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.hesvh.cn/Article/details/gdhrfrqzi.sHtML

[Q74] 强制使用索引
来源：http://blog.hesvh.cn/Article/details/gbajuyhww.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.zdbjq.cn/Article/details/gzukyvimo.sHtML

[Q75] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/gonwqwajg.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/guemigxyo.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.hesvh.cn/Article/details/gvcangiay.sHtML

[Q76] 按天统计
来源：http://blog.fehbvm.com/Article/details/gcqdhlqpm.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fehbvm.com/Article/details/gibosfpii.sHtML

[Q77] 时间加减
来源：http://baike.zdbjq.cn/Article/details/gcrohekah.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.zdbjq.cn/Article/details/gvjyzamca.sHtML

[Q78] 当前时间
来源：http://blog.hesvh.cn/Article/details/gxuwxneii.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.zdbjq.cn/Article/details/glhctxeee.sHtML

[Q79] 字符串拼接
来源：http://3g.hesvh.cn/Article/details/gxxtvhumw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fehbvm.com/Article/details/ghjsdqtze.sHtML

[Q80] 字符串截取
来源：http://www.blog.hesvh.cn/Article/details/gosstcfqr.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gxpjnduoz.sHtML

[Q81] 字符串替换
来源：http://mobile.zdbjq.cn/Article/details/glanzsgfs.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.hesvh.cn/Article/details/gacqefspb.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.hesvh.cn/Article/details/gfximxkqc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gmqqrbqhk.sHtML

[Q83] 大小写转换
来源：http://blog.fehbvm.com/Article/details/gxjtkvufi.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gpiancgef.sHtML

[Q84] 去除首尾空格
来源：http://mobile.hesvh.cn/Article/details/gkihsrkwa.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/guvmhsdlt.sHtML

[Q85] 数值取整
来源：http://www.blog.hesvh.cn/Article/details/gkwrmisyo.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fehbvm.com/Article/details/glgnalopq.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.zdbjq.cn/Article/details/gbnrdojzc.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.zdbjq.cn/Article/details/gaaxbqxrh.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.hesvh.cn/Article/details/gursoudwq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.hesvh.cn/Article/details/glbdvvsxl.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.hesvh.cn/Article/details/gmrodfoty.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.hesvh.cn/Article/details/gactzmkur.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.hesvh.cn/Article/details/gcckezoqm.sHtML

[Q89] 判断表是否存在
来源：http://mobile.zdbjq.cn/Article/details/gdhworjiv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.zdbjq.cn/Article/details/gsbaqywwc.sHtML

[Q90] 生成序号列
来源：http://wap.zdbjq.cn/Article/details/gozdkpldv.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.hesvh.cn/Article/details/gzhisvdsl.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/grnyndcin.sHtML

R. Bash 专题
来源：http://baike.hesvh.cn/Article/details/grfxjywtk.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gcbntojyb.sHtML

[R01] shebang 与严格模式
来源：http://baike.hesvh.cn/Article/details/gnrhrxdbv.sHtML

#!/usr/bin/env bash
来源：http://blog.hesvh.cn/Article/details/gizyjkudf.sHtML

set -euo pipefail
来源：http://read.share.fehbvm.com/Article/details/gygjaybra.sHtML

[R02] 变量赋值与使用
来源：http://baike.zdbjq.cn/Article/details/gaukzpict.sHtML

name="Tom"; echo "$name"
来源：http://wap.zdbjq.cn/Article/details/gckgrblzg.sHtML

[R03] 只读变量
来源：http://blog.zdbjq.cn/Article/details/geuipyxya.sHtML

readonly PI=3.14
来源：http://www.share.hesvh.cn/Article/details/gdbltjnym.sHtML

[R04] 位置参数
来源：http://blog.fehbvm.com/Article/details/gyappezbz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fehbvm.com/Article/details/glxfnwthp.sHtML

[R05] 参数默认值
来源：http://www.m.share.zdbjq.cn/Article/details/gqfgyqjcb.sHtML

name="${1:-default}"
来源：http://wap.fehbvm.com/Article/details/gclkqlbfh.sHtML

[R06] 判断命令是否存在
来源：http://3g.hesvh.cn/Article/details/gshyibofo.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/gyemqimpr.sHtML

[R07] if 判断文件
来源：http://wap.fehbvm.com/Article/details/ggxczukbu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fehbvm.com/Article/details/gemiwyznu.sHtML

[R08] 数值比较
来源：http://www.share.hesvh.cn/Article/details/ggytzecig.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.zdbjq.cn/Article/details/gzjmtshmr.sHtML

[R09] 字符串比较
来源：http://3g.hesvh.cn/Article/details/gvlhhzobh.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.zdbjq.cn/Article/details/gbnjnvwdn.sHtML

[R10] 正则匹配
来源：http://www.share.hesvh.cn/Article/details/geometuyl.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.hesvh.cn/Article/details/gtmsfvnof.sHtML

[R11] case 多分支
来源：http://www.m.share.zdbjq.cn/Article/details/gpyqfkccq.sHtML

case "$1" in
来源：http://baike.fehbvm.com/Article/details/ginuqouub.sHtML

start) echo "启动" ;;
来源：http://baike.fehbvm.com/Article/details/gikjrqoru.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.hesvh.cn/Article/details/gwuhvekfw.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.hesvh.cn/Article/details/gnlorekll.sHtML

esac
来源：http://m.share.fehbvm.com/Article/details/gvvvyfcoz.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fehbvm.com/Article/details/gwawxmikf.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.zdbjq.cn/Article/details/gnvlpikdu.sHtML

[R13] for 计数循环
来源：http://m.share.fehbvm.com/Article/details/gblukcoos.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/gnitaxpqf.sHtML

[R14] C 风格 for
来源：http://wap.zdbjq.cn/Article/details/gepqsvjgy.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/giivmjhjp.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gtsdiayrl.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.zdbjq.cn/Article/details/gcchvvitf.sHtML

[R16] until 等待条件
来源：http://baike.zdbjq.cn/Article/details/gsrdatqjx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.hesvh.cn/Article/details/gsoyocgly.sHtML

[R17] 数组定义与取值
来源：http://wap.hesvh.cn/Article/details/gvydgbxrf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.zdbjq.cn/Article/details/ginskefmo.sHtML

[R18] 遍历数组
来源：http://www.blog.fehbvm.com/Article/details/gjwwzklcb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.hesvh.cn/Article/details/gtjjnoqur.sHtML

[R19] 数组长度
来源：http://m.share.zdbjq.cn/Article/details/gpswavjjm.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gxhplmlsf.sHtML

[R20] 关联数组（字典）
来源：http://mobile.zdbjq.cn/Article/details/glbipepte.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.hesvh.cn/Article/details/ggwpfozat.sHtML

[R21] 字符串长度
来源：http://mobile.fehbvm.com/Article/details/gjdsnxluj.sHtML

echo "${#s}"
来源：http://baike.hesvh.cn/Article/details/ghqohqhtx.sHtML

[R22] 截取子串
来源：http://www.share.fehbvm.com/Article/details/gpehmneik.sHtML

echo "${s:0:5}"
来源：http://m.share.hesvh.cn/Article/details/gxeztihee.sHtML

[R23] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/gmumgryth.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.hesvh.cn/Article/details/grgkabait.sHtML

[R24] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/gqruvirbl.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.hesvh.cn/Article/details/gaonywtgm.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.zdbjq.cn/Article/details/gviptssgr.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.hesvh.cn/Article/details/geidizqts.sHtML

[R26] 命令替换
来源：http://www.blog.fehbvm.com/Article/details/gakptiori.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.zdbjq.cn/Article/details/gsvjevzrp.sHtML

[R27] 算术展开
来源：http://www.blog.hesvh.cn/Article/details/gaqwczmpp.sHtML

echo $((1 + 2 * 3))
来源：http://wap.zdbjq.cn/Article/details/gkkrknakq.sHtML

[R28] 浮点运算
来源：http://baike.hesvh.cn/Article/details/gprabhjzj.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fehbvm.com/Article/details/gtduhkgpz.sHtML

[R29] 定义函数
来源：http://3g.fehbvm.com/Article/details/gsjgqedjz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fehbvm.com/Article/details/gtrwrysba.sHtML

[R30] 函数返回状态码
来源：http://m.share.hesvh.cn/Article/details/gqumvuxti.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fehbvm.com/Article/details/gidhxjycg.sHtML

[R31] 局部变量
来源：http://www.share.fehbvm.com/Article/details/gnpuliyyo.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.hesvh.cn/Article/details/gorrnilpg.sHtML

[R32] 参数个数校验
来源：http://www.blog.zdbjq.cn/Article/details/grtbvbmcn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/gjuyuebqz.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fehbvm.com/Article/details/gndfthvxo.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fehbvm.com/Article/details/gdioltfrj.sHtML

[R34] 退出时清理
来源：http://m.share.fehbvm.com/Article/details/gqmazytas.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/gwcpksurc.sHtML

[R35] 后台执行并等待
来源：http://mobile.fehbvm.com/Article/details/gcqjymrku.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.zdbjq.cn/Article/details/gcfeezgoa.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fehbvm.com/Article/details/ggvekmrgf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.zdbjq.cn/Article/details/gcaubduqq.sHtML

[R37] 把输出赋给变量
来源：http://3g.zdbjq.cn/Article/details/gdycsqtmg.sHtML

files=$(ls -1)
来源：http://baike.hesvh.cn/Article/details/gwyoiiaxj.sHtML

[R38] 管道串联
来源：http://m.share.zdbjq.cn/Article/details/gxrkabcxc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.zdbjq.cn/Article/details/gkzxztzda.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.hesvh.cn/Article/details/gvffzlbpx.sHtML

cmd > out.log 2>&1
来源：http://read.share.zdbjq.cn/Article/details/gjglzfofa.sHtML

[R40] 追加写日志
来源：http://www.share.fehbvm.com/Article/details/ghunhnmqv.sHtML

echo "log" >> out.log
来源：http://mobile.fehbvm.com/Article/details/gtxtmbdjy.sHtML

[R41] 丢弃输出
来源：http://3g.hesvh.cn/Article/details/ggpvsfjbn.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.zdbjq.cn/Article/details/ghznfhnac.sHtML

[R42] 输入重定向
来源：http://www.share.zdbjq.cn/Article/details/gpmfvrxws.sHtML

wc -l < a.txt
来源：http://wap.zdbjq.cn/Article/details/gfmxywpzi.sHtML

[R43] 按名字查找文件
来源：http://m.share.hesvh.cn/Article/details/gquobaliu.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fehbvm.com/Article/details/gifghzbsd.sHtML

[R44] 按修改时间查找
来源：http://blog.zdbjq.cn/Article/details/gqhekegue.sHtML

find . -mtime -7 -type f
来源：http://www.blog.zdbjq.cn/Article/details/gwziwdmce.sHtML

[R45] 批量删除
来源：http://wap.hesvh.cn/Article/details/gueqdjfnf.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fehbvm.com/Article/details/gtqgwplks.sHtML

[R46] 递归替换文件内容
来源：http://wap.hesvh.cn/Article/details/gqjzphhiu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fehbvm.com/Article/details/gwbeycfyc.sHtML

[R47] sed 单行替换
来源：http://blog.zdbjq.cn/Article/details/gmlmuyhvh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.hesvh.cn/Article/details/gznsjgwzo.sHtML

[R48] awk 取指定列
来源：http://read.share.zdbjq.cn/Article/details/gnqjmcfwn.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.hesvh.cn/Article/details/gsmlsnnbk.sHtML

[R49] awk 带条件
来源：http://3g.fehbvm.com/Article/details/gykjffyrd.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.hesvh.cn/Article/details/gfddotvtc.sHtML

[R50] awk 求和
来源：http://blog.hesvh.cn/Article/details/ghnvgelmq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gjkjtlzne.sHtML

[R51] 排序去重取前几
来源：http://3g.zdbjq.cn/Article/details/ggzdonfho.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.zdbjq.cn/Article/details/grroxeqga.sHtML

[R52] 统计行数
来源：http://mobile.hesvh.cn/Article/details/gmmjvwtam.sHtML

wc -l a.txt
来源：http://m.share.fehbvm.com/Article/details/gnjngntil.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.hesvh.cn/Article/details/gsqkekghw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fehbvm.com/Article/details/gyrrxlaeo.sHtML

[R54] 比较两个文件
来源：http://read.share.hesvh.cn/Article/details/gdissavke.sHtML

diff a.txt b.txt
来源：http://baike.fehbvm.com/Article/details/grzullaxa.sHtML

[R55] 压缩与解压
来源：http://3g.hesvh.cn/Article/details/gikdmbrdw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fehbvm.com/Article/details/gurstjzhk.sHtML

[R56] 远程拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gkkcxdlpn.sHtML

scp file user@host:/path/
来源：http://www.m.share.fehbvm.com/Article/details/gdjxkcxok.sHtML

[R57] 远程执行命令
来源：http://3g.hesvh.cn/Article/details/gnqwkzxhf.sHtML

ssh user@host 'uptime'
来源：http://read.share.hesvh.cn/Article/details/ggdqtpoyt.sHtML

[R58] 下载文件
来源：http://baike.zdbjq.cn/Article/details/gobdabpwe.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.hesvh.cn/Article/details/guesmgajj.sHtML

[R59] 发 POST JSON
来源：http://mobile.fehbvm.com/Article/details/gjeeevftq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fehbvm.com/Article/details/grcauxkjf.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.hesvh.cn/Article/details/gypulzvrv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fehbvm.com/Article/details/gyznzzofa.sHtML

[R61] 磁盘占用
来源：http://wap.fehbvm.com/Article/details/gdepchmfr.sHtML

df -h;  du -sh *
来源：http://read.share.fehbvm.com/Article/details/gcxojvydm.sHtML

[R62] 找最占空间的文件
来源：http://m.share.hesvh.cn/Article/details/gaukycdun.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fehbvm.com/Article/details/geudbrdsq.sHtML

[R63] 内存与进程
来源：http://www.blog.hesvh.cn/Article/details/gviglqlyi.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.hesvh.cn/Article/details/gugfesnym.sHtML

[R64] 结束进程
来源：http://www.blog.hesvh.cn/Article/details/gcqnhorwd.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.zdbjq.cn/Article/details/gefjlwpjb.sHtML

[R65] 查看端口占用
来源：http://wap.zdbjq.cn/Article/details/gkujctkge.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.zdbjq.cn/Article/details/gbmiktdwg.sHtML

[R66] 定时任务
来源：http://www.share.zdbjq.cn/Article/details/gioilkfqm.sHtML

crontab -e;  crontab -l
来源：http://www.share.hesvh.cn/Article/details/gcxmjnkkb.sHtML

[R67] 生成随机十六进制串
来源：http://wap.zdbjq.cn/Article/details/guhxscctq.sHtML

openssl rand -hex 16
来源：http://mobile.fehbvm.com/Article/details/ggfolynhn.sHtML

[R68] 计算文件校验值
来源：http://mobile.hesvh.cn/Article/details/gwfsbnkhm.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fehbvm.com/Article/details/gwqvdvuwd.sHtML

[R69] 生成随机密码
来源：http://www.share.fehbvm.com/Article/details/ggtqliwpz.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fehbvm.com/Article/details/gvfdjoump.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.hesvh.cn/Article/details/gjfzujmnp.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.hesvh.cn/Article/details/gneamwemo.sHtML

[R71] 日期格式化
来源：http://wap.hesvh.cn/Article/details/gbuqvtlvw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.hesvh.cn/Article/details/gulhdjlfy.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.hesvh.cn/Article/details/gbhnxioeh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/gaufadqqy.sHtML

[R73] 分割大日志
来源：http://www.m.share.fehbvm.com/Article/details/gssxbjqrf.sHtML

split -l 1000 big.log part_
来源：http://baike.fehbvm.com/Article/details/gjokffvfg.sHtML

[R74] 批量重命名
来源：http://3g.zdbjq.cn/Article/details/ggqouibsy.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fehbvm.com/Article/details/ggvlncqhy.sHtML

[R75] 导出环境变量
来源：http://m.share.hesvh.cn/Article/details/gpwfeaqch.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fehbvm.com/Article/details/gridtacjh.sHtML

[R76] 使用临时文件
来源：http://wap.zdbjq.cn/Article/details/gguqhydkm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.zdbjq.cn/Article/details/gvfwyzttp.sHtML

[R77] 读取用户输入
来源：http://baike.zdbjq.cn/Article/details/gcaijfqig.sHtML

read -rp "请输入: " ans
来源：http://www.blog.zdbjq.cn/Article/details/gtzpzinuk.sHtML

[R78] 交互式菜单
来源：http://mobile.zdbjq.cn/Article/details/gnzddfswh.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.hesvh.cn/Article/details/gayqnedug.sHtML

[R79] 解析命令行选项
来源：http://m.share.zdbjq.cn/Article/details/gnucqscat.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.zdbjq.cn/Article/details/gzfzisyqz.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.hesvh.cn/Article/details/gnvbcoypp.sHtML

time ./run.sh
来源：http://3g.hesvh.cn/Article/details/ghxtycwvn.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gpmkmtvkq.sHtML

S. C / C++ 专题
来源：http://www.blog.fehbvm.com/Article/details/gmnghmhvk.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gxfuuvqfv.sHtML

[S01] C：Hello World
来源：http://www.share.hesvh.cn/Article/details/gqqgerozt.sHtML

#include <stdio.h>
来源：http://www.m.share.fehbvm.com/Article/details/gzaedruer.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fehbvm.com/Article/details/gxqxksrbe.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.hesvh.cn/Article/details/glqhiqwkv.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fehbvm.com/Article/details/gwrbbiiwe.sHtML

[S03] C：读入整数
来源：http://mobile.fehbvm.com/Article/details/ghyhgejds.sHtML

int x; scanf("%d", &x);
来源：http://mobile.zdbjq.cn/Article/details/gdiwqthex.sHtML

[S04] C：字符串复制
来源：http://baike.fehbvm.com/Article/details/gunurjibs.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gtlmzvtkd.sHtML

[S05] C：字符串长度
来源：http://baike.fehbvm.com/Article/details/gffzeqqnv.sHtML

strlen(s)
来源：http://read.share.fehbvm.com/Article/details/gzvfhudze.sHtML

[S06] C：字符串比较
来源：http://wap.zdbjq.cn/Article/details/guzhlfbdo.sHtML

strcmp(a, b) == 0
来源：http://www.share.hesvh.cn/Article/details/gxclmwvra.sHtML

[S07] C：数组遍历求和
来源：http://3g.fehbvm.com/Article/details/gxpgdrpeq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fehbvm.com/Article/details/guwwqyzru.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.hesvh.cn/Article/details/grtylfaqe.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.hesvh.cn/Article/details/geebspvnh.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.zdbjq.cn/Article/details/ghqvgkswz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.hesvh.cn/Article/details/gtdbcalgy.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fehbvm.com/Article/details/gjdweaqle.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.hesvh.cn/Article/details/gempjverq.sHtML

[S11] C：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gufeywyrb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.hesvh.cn/Article/details/gdchdnhgp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.zdbjq.cn/Article/details/gpyhdycds.sHtML

fclose(f);
来源：http://baike.hesvh.cn/Article/details/gxmsrwjne.sHtML

[S12] C：写文件
来源：http://wap.zdbjq.cn/Article/details/gbqlbufdl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fehbvm.com/Article/details/gyvdnfwee.sHtML

[S13] C：宏定义
来源：http://wap.fehbvm.com/Article/details/gifamkiim.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.hesvh.cn/Article/details/gcxhwjzdf.sHtML

[S14] C：枚举
来源：http://www.share.zdbjq.cn/Article/details/gobauuijm.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fehbvm.com/Article/details/gfoparoyr.sHtML

[S15] C：类型转换
来源：http://3g.zdbjq.cn/Article/details/giqkjesvc.sHtML

(double) a / b
来源：http://www.share.zdbjq.cn/Article/details/goitqtbwf.sHtML

[S16] C：位操作置位
来源：http://read.share.fehbvm.com/Article/details/gefifcdmq.sHtML

x |= (1 << 3);
来源：http://www.blog.fehbvm.com/Article/details/ghuxnrxeq.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fehbvm.com/Article/details/gcdkllqko.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.zdbjq.cn/Article/details/gqmkzfxnz.sHtML

[S18] C：命令行参数
来源：http://www.share.fehbvm.com/Article/details/gjprkvvmq.sHtML


<!-- 参考信息 -->