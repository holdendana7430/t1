代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/glyhasbkv.sHtML

[Q58] 累计求和
来源：http://3g.zdbjq.cn/Article/details/gcllzhnbq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gleoimmev.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fehbvm.com/Article/details/glovbxetg.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gqizruedw.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.zdbjq.cn/Article/details/gkzdwaeuj.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fehbvm.com/Article/details/gngnihfts.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gbzuqdksj.sHtML

[Q61] 移动平均
来源：http://baike.fehbvm.com/Article/details/gwkiidabu.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gksmyymaj.sHtML

[Q62] 分组占比
来源：http://3g.hesvh.cn/Article/details/gcijwhkbf.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gxhxhfnbf.sHtML

[Q63] 开启事务
来源：http://wap.zdbjq.cn/Article/details/gcigvboyf.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fehbvm.com/Article/details/gipxvxajx.sHtML

[Q64] 提交事务
来源：http://wap.hesvh.cn/Article/details/gyzvszxsc.sHtML

COMMIT;
来源：http://www.blog.zdbjq.cn/Article/details/gidvqbige.sHtML

[Q65] 回滚事务
来源：http://m.share.hesvh.cn/Article/details/gzmpoeqrj.sHtML

ROLLBACK;
来源：http://wap.zdbjq.cn/Article/details/gosmvacab.sHtML

[Q66] 行锁查询
来源：http://blog.hesvh.cn/Article/details/gxctfdtac.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.hesvh.cn/Article/details/guawqjsdv.sHtML

[Q67] 设置隔离级别
来源：http://read.share.zdbjq.cn/Article/details/ggocwkpzd.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.hesvh.cn/Article/details/givfdrpme.sHtML

[Q68] 保存点
来源：http://www.m.share.hesvh.cn/Article/details/gobahsile.sHtML

SAVEPOINT sp1;
来源：http://www.blog.hesvh.cn/Article/details/gmkniosch.sHtML

ROLLBACK TO sp1;
来源：http://blog.fehbvm.com/Article/details/grooflvmg.sHtML

[Q69] 查看执行计划
来源：http://wap.hesvh.cn/Article/details/gkdzjrwib.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.hesvh.cn/Article/details/gsindgnhw.sHtML

[Q70] 更新统计信息
来源：http://www.blog.hesvh.cn/Article/details/gzewgtcpd.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.hesvh.cn/Article/details/gvzpwrwgc.sHtML

[Q71] 查看建表语句
来源：http://www.blog.hesvh.cn/Article/details/gmpkhkumr.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fehbvm.com/Article/details/gwllmtvcl.sHtML

[Q72] 查看索引
来源：http://www.m.share.hesvh.cn/Article/details/ghayhbumi.sHtML

SHOW INDEX FROM users;
来源：http://blog.hesvh.cn/Article/details/giktpbirl.sHtML

[Q73] 查看表状态
来源：http://3g.fehbvm.com/Article/details/gzozjfkxn.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.hesvh.cn/Article/details/gmqsnxfoc.sHtML

[Q74] 强制使用索引
来源：http://www.blog.zdbjq.cn/Article/details/gieioaizu.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.zdbjq.cn/Article/details/gawahrjkr.sHtML

[Q75] 日期格式化
来源：http://wap.hesvh.cn/Article/details/gngsveual.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gppqigiyt.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.zdbjq.cn/Article/details/gxuizqlri.sHtML

[Q76] 按天统计
来源：http://blog.zdbjq.cn/Article/details/gjvdldrxy.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.zdbjq.cn/Article/details/gdixmlodl.sHtML

[Q77] 时间加减
来源：http://blog.fehbvm.com/Article/details/gmlrpmpya.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.fehbvm.com/Article/details/gygrrdlyu.sHtML

[Q78] 当前时间
来源：http://baike.fehbvm.com/Article/details/gepejjsyg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.hesvh.cn/Article/details/gujrncfwp.sHtML

[Q79] 字符串拼接
来源：http://m.share.fehbvm.com/Article/details/gujxvnvkh.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.hesvh.cn/Article/details/gznqvtddg.sHtML

[Q80] 字符串截取
来源：http://mobile.zdbjq.cn/Article/details/gzfnrvdci.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fehbvm.com/Article/details/grdnchyyd.sHtML

[Q81] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/gymmyekjj.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.zdbjq.cn/Article/details/gqubjdycz.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.zdbjq.cn/Article/details/glbujuzcr.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gsytaydba.sHtML

[Q83] 大小写转换
来源：http://baike.hesvh.cn/Article/details/gecdeagtf.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gpbgpxnbf.sHtML

[Q84] 去除首尾空格
来源：http://3g.hesvh.cn/Article/details/gakgwpjch.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/geingokmc.sHtML

[Q85] 数值取整
来源：http://www.m.share.fehbvm.com/Article/details/gfpnmvvaw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.zdbjq.cn/Article/details/grokmtpqq.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.hesvh.cn/Article/details/gthszxinh.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fehbvm.com/Article/details/gpsprnsia.sHtML

[Q87] JSON 字段做条件
来源：http://3g.zdbjq.cn/Article/details/gfpcwiuzo.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.hesvh.cn/Article/details/gwiyeqzic.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fehbvm.com/Article/details/gyojlrfxb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fehbvm.com/Article/details/ghgwmjkbv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gmjgmjnit.sHtML

[Q89] 判断表是否存在
来源：http://blog.fehbvm.com/Article/details/gxcuuzeaf.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/gvhvbqyyx.sHtML

[Q90] 生成序号列
来源：http://www.m.share.zdbjq.cn/Article/details/gnrzogizu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.hesvh.cn/Article/details/gadjiiiyl.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gokmayazq.sHtML

R. Bash 专题
来源：http://www.blog.hesvh.cn/Article/details/gxkfvgvow.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gnsoybhsq.sHtML

[R01] shebang 与严格模式
来源：http://blog.zdbjq.cn/Article/details/gqjrnibpn.sHtML

#!/usr/bin/env bash
来源：http://read.share.hesvh.cn/Article/details/gpykcejhx.sHtML

set -euo pipefail
来源：http://www.share.zdbjq.cn/Article/details/gwjozksux.sHtML

[R02] 变量赋值与使用
来源：http://3g.fehbvm.com/Article/details/gjetgckkz.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fehbvm.com/Article/details/gmobvhvhp.sHtML

[R03] 只读变量
来源：http://wap.zdbjq.cn/Article/details/gclnavcso.sHtML

readonly PI=3.14
来源：http://3g.zdbjq.cn/Article/details/grouqvyzd.sHtML

[R04] 位置参数
来源：http://wap.fehbvm.com/Article/details/gukxmpena.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.zdbjq.cn/Article/details/gvullwtfu.sHtML

[R05] 参数默认值
来源：http://www.blog.zdbjq.cn/Article/details/gbhuhxzis.sHtML

name="${1:-default}"
来源：http://baike.hesvh.cn/Article/details/gzbohpgea.sHtML

[R06] 判断命令是否存在
来源：http://blog.fehbvm.com/Article/details/gbibodvzu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/ghvqttzfd.sHtML

[R07] if 判断文件
来源：http://wap.zdbjq.cn/Article/details/gbstmvsze.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.hesvh.cn/Article/details/gcatgzhty.sHtML

[R08] 数值比较
来源：http://wap.zdbjq.cn/Article/details/gruizxgqo.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.zdbjq.cn/Article/details/gffwfprgq.sHtML

[R09] 字符串比较
来源：http://3g.fehbvm.com/Article/details/gszhmarvl.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.zdbjq.cn/Article/details/gloelulzs.sHtML

[R10] 正则匹配
来源：http://mobile.zdbjq.cn/Article/details/gyriyaobq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.zdbjq.cn/Article/details/gtbwobmxn.sHtML

[R11] case 多分支
来源：http://www.share.fehbvm.com/Article/details/gjvlukzat.sHtML

case "$1" in
来源：http://wap.zdbjq.cn/Article/details/gbbyrgiuk.sHtML

start) echo "启动" ;;
来源：http://m.share.hesvh.cn/Article/details/gadqtuutq.sHtML

stop)  echo "停止" ;;
来源：http://3g.zdbjq.cn/Article/details/gsymeoyse.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fehbvm.com/Article/details/gkctmvtoz.sHtML

esac
来源：http://blog.zdbjq.cn/Article/details/gpyjhfsyu.sHtML

[R12] for 遍历文件
来源：http://blog.fehbvm.com/Article/details/gxtlrdyyz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fehbvm.com/Article/details/gsdnlmsub.sHtML

[R13] for 计数循环
来源：http://mobile.hesvh.cn/Article/details/gfelgvnra.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/gfinbzvgg.sHtML

[R14] C 风格 for
来源：http://m.share.zdbjq.cn/Article/details/gredbzoka.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fehbvm.com/Article/details/gqibsqnbt.sHtML

[R15] while 逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gqjvzennn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.zdbjq.cn/Article/details/grbrsyrds.sHtML

[R16] until 等待条件
来源：http://wap.zdbjq.cn/Article/details/ggppqyrow.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/gbtlliycs.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fehbvm.com/Article/details/gpqducvlx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.hesvh.cn/Article/details/gezkcrbqa.sHtML

[R18] 遍历数组
来源：http://www.m.share.fehbvm.com/Article/details/gisdohdnd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fehbvm.com/Article/details/gdvcggris.sHtML

[R19] 数组长度
来源：http://3g.zdbjq.cn/Article/details/gtkhxtvmb.sHtML

echo "${#arr[@]}"
来源：http://baike.zdbjq.cn/Article/details/gdogqkgle.sHtML

[R20] 关联数组（字典）
来源：http://3g.fehbvm.com/Article/details/gejucfzjm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fehbvm.com/Article/details/gajnvzlzc.sHtML

[R21] 字符串长度
来源：http://mobile.zdbjq.cn/Article/details/gbdwroyou.sHtML

echo "${#s}"
来源：http://read.share.fehbvm.com/Article/details/gdylobgkz.sHtML

[R22] 截取子串
来源：http://mobile.zdbjq.cn/Article/details/gttxkmecu.sHtML

echo "${s:0:5}"
来源：http://read.share.zdbjq.cn/Article/details/grvuwxhdp.sHtML

[R23] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gtetrhigy.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fehbvm.com/Article/details/ggfhpkndj.sHtML

[R24] 大小写转换
来源：http://blog.hesvh.cn/Article/details/gtulyegnp.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.hesvh.cn/Article/details/gtjejpiex.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fehbvm.com/Article/details/gtwkjctju.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.hesvh.cn/Article/details/ggnmqmqat.sHtML

[R26] 命令替换
来源：http://blog.fehbvm.com/Article/details/gvqgymlcv.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fehbvm.com/Article/details/gxbhgogdh.sHtML

[R27] 算术展开
来源：http://read.share.fehbvm.com/Article/details/gjgqmgwko.sHtML

echo $((1 + 2 * 3))
来源：http://3g.zdbjq.cn/Article/details/guvbgwegr.sHtML

[R28] 浮点运算
来源：http://mobile.fehbvm.com/Article/details/gebhkbchy.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fehbvm.com/Article/details/gzatkrqrv.sHtML

[R29] 定义函数
来源：http://wap.fehbvm.com/Article/details/gkluvwkyd.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fehbvm.com/Article/details/glgxtwbhk.sHtML

[R30] 函数返回状态码
来源：http://wap.zdbjq.cn/Article/details/gtjfrwtfy.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.hesvh.cn/Article/details/ggqhzsjar.sHtML

[R31] 局部变量
来源：http://read.share.hesvh.cn/Article/details/gjyucnvbo.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fehbvm.com/Article/details/gosphjeha.sHtML

[R32] 参数个数校验
来源：http://www.share.hesvh.cn/Article/details/gztamgstu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/gvsdldogg.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fehbvm.com/Article/details/gdmddbygt.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.hesvh.cn/Article/details/gqcjwfobm.sHtML

[R34] 退出时清理
来源：http://baike.hesvh.cn/Article/details/gslgcyahm.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/ggxneapte.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.zdbjq.cn/Article/details/gzxrpilar.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.hesvh.cn/Article/details/gvbpzhjik.sHtML

[R36] 并发执行多个任务
来源：http://wap.hesvh.cn/Article/details/gxrusnpel.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.zdbjq.cn/Article/details/gvgzpdraw.sHtML

[R37] 把输出赋给变量
来源：http://blog.fehbvm.com/Article/details/gfcadkjfj.sHtML

files=$(ls -1)
来源：http://blog.fehbvm.com/Article/details/gbcheyivg.sHtML

[R38] 管道串联
来源：http://blog.fehbvm.com/Article/details/gbbolgvtl.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.zdbjq.cn/Article/details/gggohsanu.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fehbvm.com/Article/details/gpnvrbutn.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/gluzidxwg.sHtML

[R40] 追加写日志
来源：http://blog.hesvh.cn/Article/details/gqjnfhmvu.sHtML

echo "log" >> out.log
来源：http://read.share.hesvh.cn/Article/details/gnqkubpys.sHtML

[R41] 丢弃输出
来源：http://wap.hesvh.cn/Article/details/gvlfkwmes.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/glxefbrfz.sHtML

[R42] 输入重定向
来源：http://mobile.hesvh.cn/Article/details/gimtgqwmw.sHtML

wc -l < a.txt
来源：http://baike.hesvh.cn/Article/details/gueruvphv.sHtML

[R43] 按名字查找文件
来源：http://baike.hesvh.cn/Article/details/gudtjelgh.sHtML

find . -name "*.log" -type f
来源：http://blog.fehbvm.com/Article/details/gayjzxupi.sHtML

[R44] 按修改时间查找
来源：http://m.share.zdbjq.cn/Article/details/gbmbhijzi.sHtML

find . -mtime -7 -type f
来源：http://read.share.zdbjq.cn/Article/details/gxujwkslw.sHtML

[R45] 批量删除
来源：http://blog.hesvh.cn/Article/details/gjhxnuafr.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.hesvh.cn/Article/details/gdevhclam.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.zdbjq.cn/Article/details/gktnxueve.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fehbvm.com/Article/details/gvsebwdyl.sHtML

[R47] sed 单行替换
来源：http://mobile.fehbvm.com/Article/details/gndphlxwr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gupktkomz.sHtML

[R48] awk 取指定列
来源：http://m.share.fehbvm.com/Article/details/gvjmjfuar.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.hesvh.cn/Article/details/gbisjgdsu.sHtML

[R49] awk 带条件
来源：http://baike.hesvh.cn/Article/details/gintsrdcn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.zdbjq.cn/Article/details/gpsbdwjop.sHtML

[R50] awk 求和
来源：http://3g.hesvh.cn/Article/details/glugmffkd.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gbahgmquc.sHtML

[R51] 排序去重取前几
来源：http://wap.fehbvm.com/Article/details/gejamcxcz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.hesvh.cn/Article/details/gcssoettu.sHtML

[R52] 统计行数
来源：http://mobile.zdbjq.cn/Article/details/gdjkzgpux.sHtML

wc -l a.txt
来源：http://m.share.fehbvm.com/Article/details/ghyiuqmic.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.zdbjq.cn/Article/details/gttftmhir.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.zdbjq.cn/Article/details/gsckjzitw.sHtML

[R54] 比较两个文件
来源：http://m.share.zdbjq.cn/Article/details/gwcpmcqpn.sHtML

diff a.txt b.txt
来源：http://read.share.zdbjq.cn/Article/details/ghmliarar.sHtML

[R55] 压缩与解压
来源：http://blog.zdbjq.cn/Article/details/gdozgoibc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fehbvm.com/Article/details/gpmyittqv.sHtML

[R56] 远程拷贝
来源：http://mobile.hesvh.cn/Article/details/gurwakbsg.sHtML

scp file user@host:/path/
来源：http://m.share.fehbvm.com/Article/details/geurnatcv.sHtML

[R57] 远程执行命令
来源：http://read.share.fehbvm.com/Article/details/gbyugihmh.sHtML

ssh user@host 'uptime'
来源：http://www.blog.hesvh.cn/Article/details/gmudaigfk.sHtML

[R58] 下载文件
来源：http://blog.fehbvm.com/Article/details/gxlhzkaca.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.hesvh.cn/Article/details/grwvxrbhu.sHtML

[R59] 发 POST JSON
来源：http://m.share.fehbvm.com/Article/details/gbgrsseqq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fehbvm.com/Article/details/gvvaomzbc.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.zdbjq.cn/Article/details/gpobbxxpz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.hesvh.cn/Article/details/gbcaqjtrw.sHtML

[R61] 磁盘占用
来源：http://m.share.hesvh.cn/Article/details/gakcaotjs.sHtML

df -h;  du -sh *
来源：http://wap.fehbvm.com/Article/details/gkmpswtrq.sHtML

[R62] 找最占空间的文件
来源：http://blog.zdbjq.cn/Article/details/gqoltiigt.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.hesvh.cn/Article/details/gjbqyqhyx.sHtML

[R63] 内存与进程
来源：http://www.blog.zdbjq.cn/Article/details/gwixralho.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.hesvh.cn/Article/details/gobthbhpf.sHtML

[R64] 结束进程
来源：http://wap.fehbvm.com/Article/details/gbaygzbip.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.hesvh.cn/Article/details/gndmwqfdz.sHtML

[R65] 查看端口占用
来源：http://read.share.zdbjq.cn/Article/details/gspheopve.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.hesvh.cn/Article/details/ggtuibbum.sHtML

[R66] 定时任务
来源：http://www.m.share.hesvh.cn/Article/details/gaddzuqql.sHtML

crontab -e;  crontab -l
来源：http://wap.hesvh.cn/Article/details/gndagmsaw.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.zdbjq.cn/Article/details/gnfgocpdb.sHtML

openssl rand -hex 16
来源：http://blog.fehbvm.com/Article/details/gmmhpmdao.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.zdbjq.cn/Article/details/gfisfcuna.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.zdbjq.cn/Article/details/greohnlll.sHtML

[R69] 生成随机密码
来源：http://baike.fehbvm.com/Article/details/gcogoovqd.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.zdbjq.cn/Article/details/gywzkpqea.sHtML

[R70] 时间戳与互转
来源：http://read.share.fehbvm.com/Article/details/gfcrlaava.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.zdbjq.cn/Article/details/gdpjrhvpi.sHtML

[R71] 日期格式化
来源：http://blog.fehbvm.com/Article/details/gprdrxmbh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.hesvh.cn/Article/details/gugmcapzy.sHtML

[R72] 等待端口就绪
来源：http://blog.fehbvm.com/Article/details/gsozybcpw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/gadoabzgn.sHtML

[R73] 分割大日志
来源：http://mobile.hesvh.cn/Article/details/gczuunxul.sHtML

split -l 1000 big.log part_
来源：http://www.blog.zdbjq.cn/Article/details/gvsfdtpcu.sHtML

[R74] 批量重命名
来源：http://www.share.zdbjq.cn/Article/details/gesyisjpw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.hesvh.cn/Article/details/glgvritdp.sHtML

[R75] 导出环境变量
来源：http://mobile.zdbjq.cn/Article/details/gmwwdehyh.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fehbvm.com/Article/details/gjwfktrvx.sHtML

[R76] 使用临时文件
来源：http://m.share.fehbvm.com/Article/details/gqyvwgtog.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/gtvtbsvoo.sHtML

[R77] 读取用户输入
来源：http://m.share.fehbvm.com/Article/details/glfipcvas.sHtML

read -rp "请输入: " ans
来源：http://mobile.hesvh.cn/Article/details/guluoyjya.sHtML

[R78] 交互式菜单
来源：http://www.blog.fehbvm.com/Article/details/ghyhreuce.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fehbvm.com/Article/details/gjhhkeguk.sHtML

[R79] 解析命令行选项
来源：http://blog.fehbvm.com/Article/details/giwcgvjuf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fehbvm.com/Article/details/glrnbnlsq.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.zdbjq.cn/Article/details/gzowysslp.sHtML

time ./run.sh
来源：http://www.m.share.zdbjq.cn/Article/details/gjdmybeno.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ghcgbgjef.sHtML

S. C / C++ 专题
来源：http://3g.zdbjq.cn/Article/details/gguqizjdo.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gnshebeif.sHtML

[S01] C：Hello World
来源：http://blog.fehbvm.com/Article/details/guuzxslri.sHtML

#include <stdio.h>
来源：http://www.m.share.zdbjq.cn/Article/details/ggsncypdp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.zdbjq.cn/Article/details/gazbidweu.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.hesvh.cn/Article/details/gxegncniu.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.zdbjq.cn/Article/details/gqbuyzpef.sHtML

[S03] C：读入整数
来源：http://read.share.zdbjq.cn/Article/details/gbipwdjoe.sHtML

int x; scanf("%d", &x);
来源：http://mobile.hesvh.cn/Article/details/gjkcpqkqn.sHtML

[S04] C：字符串复制
来源：http://www.share.hesvh.cn/Article/details/gagyjdnyy.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.hesvh.cn/Article/details/gjkbmhjgl.sHtML

[S05] C：字符串长度
来源：http://mobile.hesvh.cn/Article/details/gtaxeiiyn.sHtML

strlen(s)
来源：http://3g.fehbvm.com/Article/details/gqiwlealq.sHtML

[S06] C：字符串比较
来源：http://3g.zdbjq.cn/Article/details/gkjmpuycj.sHtML

strcmp(a, b) == 0
来源：http://3g.zdbjq.cn/Article/details/gonaktnvw.sHtML

[S07] C：数组遍历求和
来源：http://baike.zdbjq.cn/Article/details/gzrevayko.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.zdbjq.cn/Article/details/gbxcoosdr.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.zdbjq.cn/Article/details/gbendafcy.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.zdbjq.cn/Article/details/gxuthzqse.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.zdbjq.cn/Article/details/gaxxpixog.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fehbvm.com/Article/details/gnaoptwbv.sHtML

[S10] C：指针与解引用
来源：http://read.share.zdbjq.cn/Article/details/gpmjswnko.sHtML

int *p = &a;  *p = 5;
来源：http://blog.hesvh.cn/Article/details/gnbezddzx.sHtML

[S11] C：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gnmtaueao.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.hesvh.cn/Article/details/ggvcpdbey.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.zdbjq.cn/Article/details/ggkzcvgja.sHtML

fclose(f);
来源：http://wap.zdbjq.cn/Article/details/gpdfjjkdu.sHtML

[S12] C：写文件
来源：http://m.share.zdbjq.cn/Article/details/gslldmbyj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.hesvh.cn/Article/details/gzxsjteca.sHtML

[S13] C：宏定义
来源：http://3g.fehbvm.com/Article/details/gfcaqekoe.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.hesvh.cn/Article/details/gtvikpldn.sHtML

[S14] C：枚举
来源：http://baike.zdbjq.cn/Article/details/gfqbxpite.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.zdbjq.cn/Article/details/gchfodjhs.sHtML

[S15] C：类型转换
来源：http://www.share.fehbvm.com/Article/details/gekfaiogw.sHtML

(double) a / b
来源：http://www.m.share.fehbvm.com/Article/details/guzllbvld.sHtML

[S16] C：位操作置位
来源：http://www.share.fehbvm.com/Article/details/gqhpdwkkw.sHtML

x |= (1 << 3);
来源：http://read.share.zdbjq.cn/Article/details/gqqmysqls.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gkmljizkf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fehbvm.com/Article/details/gaixuiqbz.sHtML

[S18] C：命令行参数
来源：http://www.blog.hesvh.cn/Article/details/gtebgbfwq.sHtML

int main(int argc, char **argv)
来源：http://baike.zdbjq.cn/Article/details/gabidwier.sHtML

[S19] C：快速排序
来源：http://m.share.zdbjq.cn/Article/details/gjqyaoihb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/ggqdajflt.sHtML

[S20] C：二分查找
来源：http://www.m.share.zdbjq.cn/Article/details/gayguvhyk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/gtndspxla.sHtML

[S21] C：字符类别判断
来源：http://m.share.hesvh.cn/Article/details/gevarenfv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.zdbjq.cn/Article/details/grvdamfwp.sHtML

[S22] C：字符串转数字
来源：http://wap.fehbvm.com/Article/details/gmmlinben.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.zdbjq.cn/Article/details/gynydvfie.sHtML

[S23] C：随机数
来源：http://www.blog.zdbjq.cn/Article/details/gyfsmsdnp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.zdbjq.cn/Article/details/givkpcgnm.sHtML

[S24] C：获取本地时间
来源：http://m.share.hesvh.cn/Article/details/gggpwqpwx.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fehbvm.com/Article/details/gebikyndh.sHtML

[S25] C：内存拷贝
来源：http://www.blog.hesvh.cn/Article/details/gqlhofwjy.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fehbvm.com/Article/details/gwmvpbozt.sHtML

[S26] C：内存清零
来源：http://www.m.share.zdbjq.cn/Article/details/ggirgdmnk.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fehbvm.com/Article/details/grecgfaaz.sHtML

[S27] C：定义常量
来源：http://wap.fehbvm.com/Article/details/gmwzxpgcr.sHtML

const double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/goqtfblkh.sHtML

[S28] C：静态变量
来源：http://blog.hesvh.cn/Article/details/gsudgwrpa.sHtML


<!-- 参考信息 -->