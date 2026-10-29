代发 wailian999

[Q61] 移动平均
来源：http://m.share.zdbjq.cn/Article/details/ggglvwilw.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gipofhzgy.sHtML

[Q62] 分组占比
来源：http://www.share.zdbjq.cn/Article/details/ggcjelacs.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/goyoufvyq.sHtML

[Q63] 开启事务
来源：http://www.m.share.fehbvm.com/Article/details/gvnlbmxyu.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.hesvh.cn/Article/details/gfascnszi.sHtML

[Q64] 提交事务
来源：http://www.m.share.fehbvm.com/Article/details/gxuuiwskl.sHtML

COMMIT;
来源：http://www.m.share.zdbjq.cn/Article/details/gogdevxbd.sHtML

[Q65] 回滚事务
来源：http://mobile.hesvh.cn/Article/details/glaokovtb.sHtML

ROLLBACK;
来源：http://www.blog.zdbjq.cn/Article/details/gwnvmgsbw.sHtML

[Q66] 行锁查询
来源：http://read.share.hesvh.cn/Article/details/gcbrynlys.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fehbvm.com/Article/details/ggcgqeaif.sHtML

[Q67] 设置隔离级别
来源：http://baike.fehbvm.com/Article/details/gyfneeieu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fehbvm.com/Article/details/gydcabzmf.sHtML

[Q68] 保存点
来源：http://www.m.share.fehbvm.com/Article/details/gqqakeplw.sHtML

SAVEPOINT sp1;
来源：http://baike.zdbjq.cn/Article/details/ghmszteae.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.hesvh.cn/Article/details/gdzpeyhai.sHtML

[Q69] 查看执行计划
来源：http://3g.hesvh.cn/Article/details/gdskipuos.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.hesvh.cn/Article/details/gryosfzwc.sHtML

[Q70] 更新统计信息
来源：http://mobile.hesvh.cn/Article/details/gvxbvwdpi.sHtML

ANALYZE TABLE users;
来源：http://3g.hesvh.cn/Article/details/gbhfahzpu.sHtML

[Q71] 查看建表语句
来源：http://m.share.zdbjq.cn/Article/details/gtdhdooxc.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fehbvm.com/Article/details/gtwxhzcqr.sHtML

[Q72] 查看索引
来源：http://3g.fehbvm.com/Article/details/gmqskxpky.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fehbvm.com/Article/details/gfwvaysdj.sHtML

[Q73] 查看表状态
来源：http://www.share.hesvh.cn/Article/details/guuqmyrkk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.hesvh.cn/Article/details/ggboqpcvi.sHtML

[Q74] 强制使用索引
来源：http://3g.fehbvm.com/Article/details/garwnxpfe.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.hesvh.cn/Article/details/gsgjycidp.sHtML

[Q75] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/ggmdxbrrq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fehbvm.com/Article/details/gdnpfueyh.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.zdbjq.cn/Article/details/gckdohcnp.sHtML

[Q76] 按天统计
来源：http://mobile.hesvh.cn/Article/details/grpduwpcn.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fehbvm.com/Article/details/gxojclbvt.sHtML

[Q77] 时间加减
来源：http://baike.hesvh.cn/Article/details/gudpfcihm.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.zdbjq.cn/Article/details/gegwmfztq.sHtML

[Q78] 当前时间
来源：http://www.m.share.hesvh.cn/Article/details/gjsnpneot.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.zdbjq.cn/Article/details/gebawuohq.sHtML

[Q79] 字符串拼接
来源：http://read.share.fehbvm.com/Article/details/gnznnazte.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.hesvh.cn/Article/details/gbayogtvm.sHtML

[Q80] 字符串截取
来源：http://blog.fehbvm.com/Article/details/gfsbikede.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gsnsvjmac.sHtML

[Q81] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/ggexrvyro.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.hesvh.cn/Article/details/gmofhimzg.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.hesvh.cn/Article/details/gyvvnzeqd.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gnvamehkc.sHtML

[Q83] 大小写转换
来源：http://blog.hesvh.cn/Article/details/gqglaqhjt.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gkhdsynjz.sHtML

[Q84] 去除首尾空格
来源：http://read.share.zdbjq.cn/Article/details/gwqkmdlug.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gtgubwdvd.sHtML

[Q85] 数值取整
来源：http://www.blog.fehbvm.com/Article/details/gpmuveiyg.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.zdbjq.cn/Article/details/gsprkoerx.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fehbvm.com/Article/details/gutlofytp.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fehbvm.com/Article/details/gsserspbx.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.hesvh.cn/Article/details/gtnqyfstr.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.hesvh.cn/Article/details/gimcyenby.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.fehbvm.com/Article/details/gepeugsis.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.zdbjq.cn/Article/details/gakqyacyl.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.zdbjq.cn/Article/details/gkotbtpxi.sHtML

[Q89] 判断表是否存在
来源：http://blog.fehbvm.com/Article/details/gfvfevspm.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.hesvh.cn/Article/details/gwzxquudq.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fehbvm.com/Article/details/gwjjnvhyn.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.hesvh.cn/Article/details/gtsyaipmp.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gjfjvkeux.sHtML

R. Bash 专题
来源：http://www.m.share.hesvh.cn/Article/details/gpwzasbdx.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gfgfuyhms.sHtML

[R01] shebang 与严格模式
来源：http://baike.fehbvm.com/Article/details/glpqyrdgc.sHtML

#!/usr/bin/env bash
来源：http://www.share.zdbjq.cn/Article/details/ggbdxxudx.sHtML

set -euo pipefail
来源：http://m.share.fehbvm.com/Article/details/ghxmbexnt.sHtML

[R02] 变量赋值与使用
来源：http://3g.zdbjq.cn/Article/details/gcvdfcilk.sHtML

name="Tom"; echo "$name"
来源：http://blog.zdbjq.cn/Article/details/giwpuwetd.sHtML

[R03] 只读变量
来源：http://3g.zdbjq.cn/Article/details/ghabqhdnb.sHtML

readonly PI=3.14
来源：http://mobile.zdbjq.cn/Article/details/gmpcuntrq.sHtML

[R04] 位置参数
来源：http://m.share.zdbjq.cn/Article/details/gbnashoua.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.zdbjq.cn/Article/details/goesrvzcy.sHtML

[R05] 参数默认值
来源：http://read.share.fehbvm.com/Article/details/ggnpvxuaz.sHtML

name="${1:-default}"
来源：http://mobile.zdbjq.cn/Article/details/giaofzhwu.sHtML

[R06] 判断命令是否存在
来源：http://3g.fehbvm.com/Article/details/gixoibifq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gyrsrzhzk.sHtML

[R07] if 判断文件
来源：http://3g.hesvh.cn/Article/details/gviymiyuy.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.zdbjq.cn/Article/details/gukzkowun.sHtML

[R08] 数值比较
来源：http://www.share.hesvh.cn/Article/details/ggbaxpega.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.hesvh.cn/Article/details/gqyzwghvs.sHtML

[R09] 字符串比较
来源：http://read.share.hesvh.cn/Article/details/ggoterdxk.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gpzeotdjk.sHtML

[R10] 正则匹配
来源：http://baike.zdbjq.cn/Article/details/gbrwzxbke.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fehbvm.com/Article/details/guuruqrxk.sHtML

[R11] case 多分支
来源：http://blog.hesvh.cn/Article/details/guertbysx.sHtML

case "$1" in
来源：http://www.share.fehbvm.com/Article/details/gripcovty.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fehbvm.com/Article/details/ggpjhdthg.sHtML

stop)  echo "停止" ;;
来源：http://blog.hesvh.cn/Article/details/gnlvaieek.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fehbvm.com/Article/details/grqijlivr.sHtML

esac
来源：http://www.m.share.zdbjq.cn/Article/details/gevsurrba.sHtML

[R12] for 遍历文件
来源：http://mobile.zdbjq.cn/Article/details/gndopwakz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fehbvm.com/Article/details/gnkskbbft.sHtML

[R13] for 计数循环
来源：http://www.share.hesvh.cn/Article/details/gadizhugd.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/gttkbecyk.sHtML

[R14] C 风格 for
来源：http://m.share.hesvh.cn/Article/details/gbhmwsegw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/glrifbsml.sHtML

[R15] while 逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gwsqueobs.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.hesvh.cn/Article/details/gmujawajc.sHtML

[R16] until 等待条件
来源：http://blog.fehbvm.com/Article/details/grcwxtear.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/gqgpsevxa.sHtML

[R17] 数组定义与取值
来源：http://mobile.zdbjq.cn/Article/details/gcmlwgzis.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.hesvh.cn/Article/details/gyypjienh.sHtML

[R18] 遍历数组
来源：http://wap.fehbvm.com/Article/details/ggizhlcyt.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.hesvh.cn/Article/details/glrytycbu.sHtML

[R19] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/gykcsmdju.sHtML

echo "${#arr[@]}"
来源：http://mobile.hesvh.cn/Article/details/gbdogpzpo.sHtML

[R20] 关联数组（字典）
来源：http://m.share.zdbjq.cn/Article/details/gnbiwlmeu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.zdbjq.cn/Article/details/gygffgmwn.sHtML

[R21] 字符串长度
来源：http://wap.zdbjq.cn/Article/details/gyvsntgka.sHtML

echo "${#s}"
来源：http://3g.hesvh.cn/Article/details/gjyvaifho.sHtML

[R22] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/gdwsuvnza.sHtML

echo "${s:0:5}"
来源：http://wap.zdbjq.cn/Article/details/gjyjkjdie.sHtML

[R23] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/gawqxztkj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fehbvm.com/Article/details/guyvmbsfd.sHtML

[R24] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/ghvmtvrai.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.hesvh.cn/Article/details/gbxnxcjix.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.hesvh.cn/Article/details/gbgnjvscy.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fehbvm.com/Article/details/gwzzebqjm.sHtML

[R26] 命令替换
来源：http://read.share.zdbjq.cn/Article/details/gueihgukm.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.hesvh.cn/Article/details/gmbdqluqy.sHtML

[R27] 算术展开
来源：http://3g.hesvh.cn/Article/details/gkkmkqcgq.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.zdbjq.cn/Article/details/gcoqbeqno.sHtML

[R28] 浮点运算
来源：http://3g.fehbvm.com/Article/details/gtmrsfvjw.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.hesvh.cn/Article/details/gplcbqrgs.sHtML

[R29] 定义函数
来源：http://blog.hesvh.cn/Article/details/gbbxwjftb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.hesvh.cn/Article/details/gwyhqynff.sHtML

[R30] 函数返回状态码
来源：http://read.share.fehbvm.com/Article/details/ghpgvspne.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.zdbjq.cn/Article/details/gqhholhcz.sHtML

[R31] 局部变量
来源：http://wap.hesvh.cn/Article/details/ghmpefhve.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.hesvh.cn/Article/details/gqsdhjezr.sHtML

[R32] 参数个数校验
来源：http://blog.fehbvm.com/Article/details/gzfuntzmz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gerkgrgey.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.hesvh.cn/Article/details/gfwajotxg.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.hesvh.cn/Article/details/gkbqzembz.sHtML

[R34] 退出时清理
来源：http://3g.fehbvm.com/Article/details/ghchsddru.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gkexelsut.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.zdbjq.cn/Article/details/gqmqzaxjc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.hesvh.cn/Article/details/ghcpryxjz.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fehbvm.com/Article/details/gsrkmhisd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.zdbjq.cn/Article/details/glzkhxzsi.sHtML

[R37] 把输出赋给变量
来源：http://read.share.zdbjq.cn/Article/details/gplawwiwk.sHtML

files=$(ls -1)
来源：http://www.blog.hesvh.cn/Article/details/gekmnhadv.sHtML

[R38] 管道串联
来源：http://www.share.hesvh.cn/Article/details/gtanawpqm.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.hesvh.cn/Article/details/gscjdpzwc.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fehbvm.com/Article/details/gpddrnkud.sHtML

cmd > out.log 2>&1
来源：http://www.share.zdbjq.cn/Article/details/gfbauegug.sHtML

[R40] 追加写日志
来源：http://www.blog.zdbjq.cn/Article/details/gkvualxsn.sHtML

echo "log" >> out.log
来源：http://wap.zdbjq.cn/Article/details/ghyrxhzug.sHtML

[R41] 丢弃输出
来源：http://wap.hesvh.cn/Article/details/gxwaginlj.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.hesvh.cn/Article/details/gwfkdgfra.sHtML

[R42] 输入重定向
来源：http://m.share.hesvh.cn/Article/details/gnorgqhih.sHtML

wc -l < a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gjuwhpjla.sHtML

[R43] 按名字查找文件
来源：http://wap.fehbvm.com/Article/details/gxglnjran.sHtML

find . -name "*.log" -type f
来源：http://blog.zdbjq.cn/Article/details/gbzbbksfc.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fehbvm.com/Article/details/grrfszxbx.sHtML

find . -mtime -7 -type f
来源：http://read.share.hesvh.cn/Article/details/glevgtlod.sHtML

[R45] 批量删除
来源：http://www.m.share.fehbvm.com/Article/details/gegvrtkwj.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.hesvh.cn/Article/details/gywuajikl.sHtML

[R46] 递归替换文件内容
来源：http://baike.zdbjq.cn/Article/details/gtblzjjml.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fehbvm.com/Article/details/goltmlcwu.sHtML

[R47] sed 单行替换
来源：http://www.share.zdbjq.cn/Article/details/gugqmbgtp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.hesvh.cn/Article/details/gcuxrtfqz.sHtML

[R48] awk 取指定列
来源：http://m.share.zdbjq.cn/Article/details/gbwdyhgjj.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gnaywkznt.sHtML

[R49] awk 带条件
来源：http://3g.fehbvm.com/Article/details/gptzzgonf.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fehbvm.com/Article/details/galliesgc.sHtML

[R50] awk 求和
来源：http://www.m.share.hesvh.cn/Article/details/ghmqfnlqk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fehbvm.com/Article/details/gegqhyuxh.sHtML

[R51] 排序去重取前几
来源：http://wap.hesvh.cn/Article/details/gdkvtvsyh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.hesvh.cn/Article/details/gabncqbxc.sHtML

[R52] 统计行数
来源：http://wap.zdbjq.cn/Article/details/gyqynaduq.sHtML

wc -l a.txt
来源：http://3g.hesvh.cn/Article/details/ghwgpnyxr.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.hesvh.cn/Article/details/ggtsuhzpc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.hesvh.cn/Article/details/gjoaccqsj.sHtML

[R54] 比较两个文件
来源：http://read.share.zdbjq.cn/Article/details/gwahgnelm.sHtML

diff a.txt b.txt
来源：http://3g.fehbvm.com/Article/details/gtxyhxeud.sHtML

[R55] 压缩与解压
来源：http://baike.hesvh.cn/Article/details/grzaybiki.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fehbvm.com/Article/details/gqlkexajl.sHtML

[R56] 远程拷贝
来源：http://blog.zdbjq.cn/Article/details/gesocbuph.sHtML

scp file user@host:/path/
来源：http://www.share.fehbvm.com/Article/details/gmxtguuop.sHtML

[R57] 远程执行命令
来源：http://read.share.hesvh.cn/Article/details/gjjkcuyaw.sHtML

ssh user@host 'uptime'
来源：http://baike.hesvh.cn/Article/details/gjrmpgmhe.sHtML

[R58] 下载文件
来源：http://3g.hesvh.cn/Article/details/gwkcslfat.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.zdbjq.cn/Article/details/gsjehbxyr.sHtML

[R59] 发 POST JSON
来源：http://www.share.zdbjq.cn/Article/details/gusgdpcdn.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.hesvh.cn/Article/details/gzuqzvgby.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/gdhrhjpvn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fehbvm.com/Article/details/gjlrxxcne.sHtML

[R61] 磁盘占用
来源：http://m.share.fehbvm.com/Article/details/gftlpxoxr.sHtML

df -h;  du -sh *
来源：http://mobile.hesvh.cn/Article/details/geuirmudl.sHtML

[R62] 找最占空间的文件
来源：http://read.share.zdbjq.cn/Article/details/gzdyaqbfp.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.hesvh.cn/Article/details/gabjtdnva.sHtML

[R63] 内存与进程
来源：http://www.m.share.zdbjq.cn/Article/details/gmjeboekq.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.hesvh.cn/Article/details/gzullwyfw.sHtML

[R64] 结束进程
来源：http://www.share.hesvh.cn/Article/details/gtmexmsap.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.zdbjq.cn/Article/details/gdfoqqhga.sHtML

[R65] 查看端口占用
来源：http://www.share.hesvh.cn/Article/details/ggrvrchff.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.zdbjq.cn/Article/details/guxeqakca.sHtML

[R66] 定时任务
来源：http://mobile.fehbvm.com/Article/details/gvilsrtjc.sHtML

crontab -e;  crontab -l
来源：http://mobile.hesvh.cn/Article/details/gwknixzmm.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fehbvm.com/Article/details/ghhdpaonv.sHtML

openssl rand -hex 16
来源：http://wap.fehbvm.com/Article/details/gfbkkklzp.sHtML

[R68] 计算文件校验值
来源：http://www.blog.zdbjq.cn/Article/details/grcbymqjs.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.hesvh.cn/Article/details/glvsmqeud.sHtML

[R69] 生成随机密码
来源：http://wap.zdbjq.cn/Article/details/gtsllfmyi.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.hesvh.cn/Article/details/ghottkulx.sHtML

[R70] 时间戳与互转
来源：http://www.share.fehbvm.com/Article/details/gojxfoyli.sHtML

date +%s;  date -d @1700000000
来源：http://baike.hesvh.cn/Article/details/gjrttnqtg.sHtML

[R71] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/ghkgwavjz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.hesvh.cn/Article/details/gpavchsgg.sHtML

[R72] 等待端口就绪
来源：http://read.share.zdbjq.cn/Article/details/gjovvipwx.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/gdpnjmtif.sHtML

[R73] 分割大日志
来源：http://wap.hesvh.cn/Article/details/gtgysxgcm.sHtML

split -l 1000 big.log part_
来源：http://baike.hesvh.cn/Article/details/gmrxotabt.sHtML

[R74] 批量重命名
来源：http://mobile.hesvh.cn/Article/details/gaarvynio.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fehbvm.com/Article/details/gqftbyphe.sHtML

[R75] 导出环境变量
来源：http://www.share.zdbjq.cn/Article/details/gkctwktsn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fehbvm.com/Article/details/gyndhcmbq.sHtML

[R76] 使用临时文件
来源：http://www.blog.fehbvm.com/Article/details/gwxctnhnb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/geylxilwk.sHtML

[R77] 读取用户输入
来源：http://3g.zdbjq.cn/Article/details/geggaajvo.sHtML

read -rp "请输入: " ans
来源：http://www.share.hesvh.cn/Article/details/gqbeltzvz.sHtML

[R78] 交互式菜单
来源：http://www.m.share.zdbjq.cn/Article/details/gttqwrzbj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fehbvm.com/Article/details/ggirrgrzu.sHtML

[R79] 解析命令行选项
来源：http://m.share.fehbvm.com/Article/details/ggrvssjht.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.zdbjq.cn/Article/details/gubiujqow.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.zdbjq.cn/Article/details/glhawdcbb.sHtML

time ./run.sh
来源：http://3g.fehbvm.com/Article/details/grcqpajdk.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gdktyddbt.sHtML

S. C / C++ 专题
来源：http://read.share.hesvh.cn/Article/details/gxhrwfzop.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gnourepmf.sHtML

[S01] C：Hello World
来源：http://read.share.fehbvm.com/Article/details/gjlugakod.sHtML

#include <stdio.h>
来源：http://www.blog.hesvh.cn/Article/details/gqixtuknq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.zdbjq.cn/Article/details/gtetbtwpe.sHtML

[S02] C：变量与格式化输出
来源：http://blog.zdbjq.cn/Article/details/goapspicu.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.hesvh.cn/Article/details/glgffgmdj.sHtML

[S03] C：读入整数
来源：http://baike.hesvh.cn/Article/details/gjvtftype.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fehbvm.com/Article/details/gdjagcbey.sHtML

[S04] C：字符串复制
来源：http://3g.fehbvm.com/Article/details/gzkxeaema.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.hesvh.cn/Article/details/gdlpktreb.sHtML

[S05] C：字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/gexltydui.sHtML

strlen(s)
来源：http://baike.hesvh.cn/Article/details/gucgmmggy.sHtML

[S06] C：字符串比较
来源：http://blog.zdbjq.cn/Article/details/gwycafiwu.sHtML

strcmp(a, b) == 0
来源：http://baike.fehbvm.com/Article/details/glejyawxu.sHtML

[S07] C：数组遍历求和
来源：http://read.share.zdbjq.cn/Article/details/gzkunspdl.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.zdbjq.cn/Article/details/gbanfhxxz.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fehbvm.com/Article/details/gugiuawlk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.zdbjq.cn/Article/details/gytxbjxlp.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.hesvh.cn/Article/details/gohklxrvm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.hesvh.cn/Article/details/gpomuctbx.sHtML

[S10] C：指针与解引用
来源：http://blog.hesvh.cn/Article/details/guxidmkoq.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fehbvm.com/Article/details/geyycfokn.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gnoneuwop.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fehbvm.com/Article/details/ggmbphpww.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fehbvm.com/Article/details/gnbzfihvz.sHtML

fclose(f);
来源：http://3g.zdbjq.cn/Article/details/gqhabptki.sHtML

[S12] C：写文件
来源：http://wap.zdbjq.cn/Article/details/gynqqxuxb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/gurzbqowl.sHtML

[S13] C：宏定义
来源：http://wap.hesvh.cn/Article/details/gcvdfrfub.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fehbvm.com/Article/details/gqxmpfbkp.sHtML

[S14] C：枚举
来源：http://baike.hesvh.cn/Article/details/gaklcekbe.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.hesvh.cn/Article/details/gxraowftd.sHtML

[S15] C：类型转换
来源：http://www.blog.hesvh.cn/Article/details/geqrkjxjz.sHtML

(double) a / b
来源：http://read.share.fehbvm.com/Article/details/gmjeabmkg.sHtML

[S16] C：位操作置位
来源：http://wap.fehbvm.com/Article/details/gzjdkhomx.sHtML

x |= (1 << 3);
来源：http://www.m.share.fehbvm.com/Article/details/gcxlclaab.sHtML

[S17] C：安全拼接字符串
来源：http://baike.hesvh.cn/Article/details/gdufwehoy.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.hesvh.cn/Article/details/giryhnwon.sHtML

[S18] C：命令行参数
来源：http://read.share.fehbvm.com/Article/details/gdnckrzll.sHtML

int main(int argc, char **argv)
来源：http://read.share.hesvh.cn/Article/details/gxdsxtggu.sHtML

[S19] C：快速排序
来源：http://www.share.fehbvm.com/Article/details/gxxvnabff.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gozusxmkc.sHtML

[S20] C：二分查找
来源：http://baike.zdbjq.cn/Article/details/gzoqhlojq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gazwgpswi.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fehbvm.com/Article/details/goxbhlbvv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.hesvh.cn/Article/details/grqemsxms.sHtML

[S22] C：字符串转数字
来源：http://www.share.fehbvm.com/Article/details/gpgqkejom.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.hesvh.cn/Article/details/gwfwecevy.sHtML

[S23] C：随机数
来源：http://www.m.share.fehbvm.com/Article/details/gdehtxmbk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fehbvm.com/Article/details/gjskpihlq.sHtML

[S24] C：获取本地时间
来源：http://read.share.zdbjq.cn/Article/details/gtguwzzod.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fehbvm.com/Article/details/grttubtfq.sHtML

[S25] C：内存拷贝
来源：http://m.share.zdbjq.cn/Article/details/gouadadii.sHtML

memcpy(dst, src, n);
来源：http://3g.zdbjq.cn/Article/details/glsenocgk.sHtML

[S26] C：内存清零
来源：http://m.share.hesvh.cn/Article/details/gtwwgcljn.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fehbvm.com/Article/details/gqyjtbkcp.sHtML

[S27] C：定义常量
来源：http://www.share.zdbjq.cn/Article/details/gzdstdpzg.sHtML

const double PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gbojiwrss.sHtML

[S28] C：静态变量
来源：http://3g.fehbvm.com/Article/details/gvmqlsywy.sHtML

static int counter = 0;
来源：http://www.blog.zdbjq.cn/Article/details/gkpzneesk.sHtML

[S29] C：变参函数
来源：http://read.share.zdbjq.cn/Article/details/ggmsuwsjh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.zdbjq.cn/Article/details/gyirnbxsl.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fehbvm.com/Article/details/gvxebhckg.sHtML

#ifndef X_H
来源：http://www.m.share.hesvh.cn/Article/details/gkmfxgtzy.sHtML

#define X_H
来源：http://read.share.zdbjq.cn/Article/details/gyuacskua.sHtML

#endif
来源：http://3g.hesvh.cn/Article/details/gxvtslaja.sHtML

[S31] C++：Hello World
来源：http://wap.hesvh.cn/Article/details/gchjqcbky.sHtML


<!-- 参考信息 -->