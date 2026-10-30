代发 wailian999

[Q61] 移动平均
来源：http://read.share.hesvh.cn/Article/details/gponledyk.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gzcmliglj.sHtML

[Q62] 分组占比
来源：http://blog.hesvh.cn/Article/details/gkbtmvphd.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/guouthxvj.sHtML

[Q63] 开启事务
来源：http://m.share.zdbjq.cn/Article/details/gacvmzond.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.hesvh.cn/Article/details/gkmsqsjub.sHtML

[Q64] 提交事务
来源：http://www.m.share.hesvh.cn/Article/details/gfkmleahi.sHtML

COMMIT;
来源：http://blog.hesvh.cn/Article/details/gmwgmhktz.sHtML

[Q65] 回滚事务
来源：http://mobile.fehbvm.com/Article/details/goamongnf.sHtML

ROLLBACK;
来源：http://read.share.fehbvm.com/Article/details/gpwlkbceh.sHtML

[Q66] 行锁查询
来源：http://3g.hesvh.cn/Article/details/gbitbvwqa.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fehbvm.com/Article/details/grlwnfugk.sHtML

[Q67] 设置隔离级别
来源：http://baike.fehbvm.com/Article/details/gbwvlbhdt.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.zdbjq.cn/Article/details/gpptfrlqh.sHtML

[Q68] 保存点
来源：http://3g.zdbjq.cn/Article/details/gzfqzhvzm.sHtML

SAVEPOINT sp1;
来源：http://www.blog.zdbjq.cn/Article/details/ghmqhahio.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/gtdnurait.sHtML

[Q69] 查看执行计划
来源：http://www.blog.fehbvm.com/Article/details/grmwktvxk.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.zdbjq.cn/Article/details/ginxwblby.sHtML

[Q70] 更新统计信息
来源：http://wap.zdbjq.cn/Article/details/guhccvfue.sHtML

ANALYZE TABLE users;
来源：http://m.share.fehbvm.com/Article/details/gewkdkgxi.sHtML

[Q71] 查看建表语句
来源：http://3g.hesvh.cn/Article/details/gjmuccqgt.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.zdbjq.cn/Article/details/gtllafcok.sHtML

[Q72] 查看索引
来源：http://m.share.fehbvm.com/Article/details/gqlwlxcmw.sHtML

SHOW INDEX FROM users;
来源：http://baike.zdbjq.cn/Article/details/gamdiijiv.sHtML

[Q73] 查看表状态
来源：http://www.share.hesvh.cn/Article/details/gzodjufcl.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fehbvm.com/Article/details/gfkrviojl.sHtML

[Q74] 强制使用索引
来源：http://baike.fehbvm.com/Article/details/gognwsjqy.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.hesvh.cn/Article/details/gifyjxkyy.sHtML

[Q75] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/gjjcwldcc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fehbvm.com/Article/details/gqrgyhlmg.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.hesvh.cn/Article/details/gycujnqgx.sHtML

[Q76] 按天统计
来源：http://3g.fehbvm.com/Article/details/gfkzuyzed.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fehbvm.com/Article/details/gsrwnauhe.sHtML

[Q77] 时间加减
来源：http://www.blog.hesvh.cn/Article/details/gfznjgvfq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.fehbvm.com/Article/details/gbkhdnpil.sHtML

[Q78] 当前时间
来源：http://www.m.share.fehbvm.com/Article/details/ghehlsjhf.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fehbvm.com/Article/details/gaxbmnbqh.sHtML

[Q79] 字符串拼接
来源：http://wap.hesvh.cn/Article/details/gfazzvdis.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.hesvh.cn/Article/details/gzrsxfeyh.sHtML

[Q80] 字符串截取
来源：http://blog.zdbjq.cn/Article/details/gxfppusko.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gkxdqmtbc.sHtML

[Q81] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/gywzypdec.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gpabsbzzf.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.hesvh.cn/Article/details/gqkicmvqz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gndhoreaw.sHtML

[Q83] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gcagvgmjb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gtclescdu.sHtML

[Q84] 去除首尾空格
来源：http://baike.fehbvm.com/Article/details/gztblyieu.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gfjtozmhy.sHtML

[Q85] 数值取整
来源：http://www.share.hesvh.cn/Article/details/giehkwfuu.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fehbvm.com/Article/details/gtpuozpjc.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.zdbjq.cn/Article/details/gsvixirps.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.hesvh.cn/Article/details/gcekfzvqn.sHtML

[Q87] JSON 字段做条件
来源：http://baike.zdbjq.cn/Article/details/gfofrkdnf.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.zdbjq.cn/Article/details/gebniegrm.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fehbvm.com/Article/details/gsxbgiosx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.hesvh.cn/Article/details/gghoopkvg.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/ghodqtvcq.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gubsljkzl.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.zdbjq.cn/Article/details/gscyqdwcd.sHtML

[Q90] 生成序号列
来源：http://mobile.fehbvm.com/Article/details/gkzozcnmy.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fehbvm.com/Article/details/gqdcbivhe.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gpfeoftrj.sHtML

R. Bash 专题
来源：http://read.share.fehbvm.com/Article/details/gapwdknmh.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gvatgvjeh.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fehbvm.com/Article/details/gcsocqtxm.sHtML

#!/usr/bin/env bash
来源：http://wap.fehbvm.com/Article/details/ghqsqiqcf.sHtML

set -euo pipefail
来源：http://read.share.hesvh.cn/Article/details/gmwynjpps.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fehbvm.com/Article/details/ggqyjxxgs.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fehbvm.com/Article/details/ggwsswmgn.sHtML

[R03] 只读变量
来源：http://www.m.share.zdbjq.cn/Article/details/gwvleaokc.sHtML

readonly PI=3.14
来源：http://www.m.share.hesvh.cn/Article/details/gjvasczpm.sHtML

[R04] 位置参数
来源：http://www.share.hesvh.cn/Article/details/gznvsrpbo.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.zdbjq.cn/Article/details/gvdygaker.sHtML

[R05] 参数默认值
来源：http://www.blog.zdbjq.cn/Article/details/gtnnkpolp.sHtML

name="${1:-default}"
来源：http://wap.fehbvm.com/Article/details/gpvtiwojv.sHtML

[R06] 判断命令是否存在
来源：http://read.share.hesvh.cn/Article/details/gbjdgukle.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/gmcusvorn.sHtML

[R07] if 判断文件
来源：http://wap.zdbjq.cn/Article/details/gsanaecpk.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.hesvh.cn/Article/details/gkoyqmcbs.sHtML

[R08] 数值比较
来源：http://mobile.fehbvm.com/Article/details/gcpngpggl.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fehbvm.com/Article/details/gazgmosel.sHtML

[R09] 字符串比较
来源：http://mobile.zdbjq.cn/Article/details/gsurgmlrx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fehbvm.com/Article/details/gqutwkbpa.sHtML

[R10] 正则匹配
来源：http://www.blog.hesvh.cn/Article/details/gskenmibu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fehbvm.com/Article/details/gtozbwyxt.sHtML

[R11] case 多分支
来源：http://mobile.fehbvm.com/Article/details/gmeruapvh.sHtML

case "$1" in
来源：http://www.m.share.fehbvm.com/Article/details/gazjigtcx.sHtML

start) echo "启动" ;;
来源：http://baike.fehbvm.com/Article/details/gejvluotw.sHtML

stop)  echo "停止" ;;
来源：http://m.share.hesvh.cn/Article/details/gsksnhogl.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.hesvh.cn/Article/details/gegxxpufo.sHtML

esac
来源：http://www.share.hesvh.cn/Article/details/gqboisaif.sHtML

[R12] for 遍历文件
来源：http://www.m.share.hesvh.cn/Article/details/gqfzbkgew.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.zdbjq.cn/Article/details/gyeogwhrv.sHtML

[R13] for 计数循环
来源：http://baike.hesvh.cn/Article/details/gmkxhmtqx.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/gcsffcjnf.sHtML

[R14] C 风格 for
来源：http://blog.zdbjq.cn/Article/details/gajamqvqv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/gtptwdnsk.sHtML

[R15] while 逐行读文件
来源：http://baike.hesvh.cn/Article/details/guiyrtlel.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.hesvh.cn/Article/details/gocgltdhr.sHtML

[R16] until 等待条件
来源：http://mobile.fehbvm.com/Article/details/givwcuskb.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/ghzfmunqx.sHtML

[R17] 数组定义与取值
来源：http://wap.hesvh.cn/Article/details/gzvpiugnu.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.hesvh.cn/Article/details/gkyvsiemn.sHtML

[R18] 遍历数组
来源：http://baike.fehbvm.com/Article/details/gifymrnmu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.zdbjq.cn/Article/details/giubbbqnr.sHtML

[R19] 数组长度
来源：http://read.share.hesvh.cn/Article/details/gzebfnydm.sHtML

echo "${#arr[@]}"
来源：http://mobile.hesvh.cn/Article/details/gcgbqltqf.sHtML

[R20] 关联数组（字典）
来源：http://read.share.zdbjq.cn/Article/details/gofauxpzo.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.zdbjq.cn/Article/details/gnhftnoaz.sHtML

[R21] 字符串长度
来源：http://read.share.zdbjq.cn/Article/details/gwkkicqzv.sHtML

echo "${#s}"
来源：http://mobile.fehbvm.com/Article/details/gljkcbcyj.sHtML

[R22] 截取子串
来源：http://mobile.hesvh.cn/Article/details/gtgdajocn.sHtML

echo "${s:0:5}"
来源：http://m.share.fehbvm.com/Article/details/gwhihvyzl.sHtML

[R23] 字符串替换
来源：http://blog.fehbvm.com/Article/details/gqmtfihgc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fehbvm.com/Article/details/gjhjjfvay.sHtML

[R24] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/gdiroaapy.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.zdbjq.cn/Article/details/gdjmezisj.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fehbvm.com/Article/details/gddfhwstd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.hesvh.cn/Article/details/guomddavy.sHtML

[R26] 命令替换
来源：http://wap.zdbjq.cn/Article/details/gqviiwgin.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.hesvh.cn/Article/details/ghbhcdjuc.sHtML

[R27] 算术展开
来源：http://3g.zdbjq.cn/Article/details/gopbmxauv.sHtML

echo $((1 + 2 * 3))
来源：http://baike.zdbjq.cn/Article/details/gjduhoazh.sHtML

[R28] 浮点运算
来源：http://mobile.zdbjq.cn/Article/details/gbjeulnbp.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fehbvm.com/Article/details/gfyilpaqq.sHtML

[R29] 定义函数
来源：http://3g.hesvh.cn/Article/details/gogsdfftn.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fehbvm.com/Article/details/guritpvka.sHtML

[R30] 函数返回状态码
来源：http://3g.hesvh.cn/Article/details/guptgcjry.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.zdbjq.cn/Article/details/gqyhcuazi.sHtML

[R31] 局部变量
来源：http://baike.hesvh.cn/Article/details/gilybzduo.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fehbvm.com/Article/details/gdeygpzsm.sHtML

[R32] 参数个数校验
来源：http://baike.zdbjq.cn/Article/details/gqtlkibzf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/ghwcejmyp.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fehbvm.com/Article/details/grxyflncd.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fehbvm.com/Article/details/gsuwpivmz.sHtML

[R34] 退出时清理
来源：http://www.m.share.zdbjq.cn/Article/details/ggbqeptji.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gvqudzbnh.sHtML

[R35] 后台执行并等待
来源：http://m.share.fehbvm.com/Article/details/guouxwpzr.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fehbvm.com/Article/details/gzalebqsq.sHtML

[R36] 并发执行多个任务
来源：http://blog.zdbjq.cn/Article/details/gkviohyir.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fehbvm.com/Article/details/gomjaqgga.sHtML

[R37] 把输出赋给变量
来源：http://blog.fehbvm.com/Article/details/grzovwtnl.sHtML

files=$(ls -1)
来源：http://www.blog.hesvh.cn/Article/details/giwfurzvh.sHtML

[R38] 管道串联
来源：http://m.share.zdbjq.cn/Article/details/gdfkewjse.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.zdbjq.cn/Article/details/geklfjbav.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.zdbjq.cn/Article/details/gewdalrfk.sHtML

cmd > out.log 2>&1
来源：http://www.share.zdbjq.cn/Article/details/gayasztkq.sHtML

[R40] 追加写日志
来源：http://www.blog.fehbvm.com/Article/details/geeaciadb.sHtML

echo "log" >> out.log
来源：http://mobile.zdbjq.cn/Article/details/gwzsvqbnv.sHtML

[R41] 丢弃输出
来源：http://3g.zdbjq.cn/Article/details/grccwvqmd.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/gonlesapu.sHtML

[R42] 输入重定向
来源：http://www.m.share.zdbjq.cn/Article/details/gaqhwwzdt.sHtML

wc -l < a.txt
来源：http://3g.hesvh.cn/Article/details/gsxsclkum.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.hesvh.cn/Article/details/gnjajhfai.sHtML

find . -name "*.log" -type f
来源：http://3g.zdbjq.cn/Article/details/goilgsopf.sHtML

[R44] 按修改时间查找
来源：http://blog.fehbvm.com/Article/details/gorwtbbhy.sHtML

find . -mtime -7 -type f
来源：http://baike.fehbvm.com/Article/details/gyvqnbpja.sHtML

[R45] 批量删除
来源：http://mobile.zdbjq.cn/Article/details/gdjgdpmeu.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.zdbjq.cn/Article/details/gwgwsfrzd.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fehbvm.com/Article/details/gmjcgkvus.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fehbvm.com/Article/details/gfbtiznar.sHtML

[R47] sed 单行替换
来源：http://read.share.fehbvm.com/Article/details/gnoefmrqo.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.hesvh.cn/Article/details/gsxksuxye.sHtML

[R48] awk 取指定列
来源：http://wap.zdbjq.cn/Article/details/gmynhmlrw.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fehbvm.com/Article/details/gwrjbckvt.sHtML

[R49] awk 带条件
来源：http://blog.zdbjq.cn/Article/details/ghfvgihcl.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.hesvh.cn/Article/details/gbpowyczl.sHtML

[R50] awk 求和
来源：http://wap.fehbvm.com/Article/details/gvhulmjdx.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fehbvm.com/Article/details/gdzpzfvji.sHtML

[R51] 排序去重取前几
来源：http://blog.zdbjq.cn/Article/details/gdfznujmc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.hesvh.cn/Article/details/gsmyawafk.sHtML

[R52] 统计行数
来源：http://wap.fehbvm.com/Article/details/gherlodpv.sHtML

wc -l a.txt
来源：http://read.share.hesvh.cn/Article/details/gxwqsqkya.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.zdbjq.cn/Article/details/gdkwnbejx.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.zdbjq.cn/Article/details/gqcnswhtc.sHtML

[R54] 比较两个文件
来源：http://wap.zdbjq.cn/Article/details/geudjdany.sHtML

diff a.txt b.txt
来源：http://www.m.share.fehbvm.com/Article/details/gfxmfkxhe.sHtML

[R55] 压缩与解压
来源：http://wap.hesvh.cn/Article/details/gpbsmqieo.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.hesvh.cn/Article/details/gdvhsaurl.sHtML

[R56] 远程拷贝
来源：http://m.share.zdbjq.cn/Article/details/gohxrscrp.sHtML

scp file user@host:/path/
来源：http://wap.fehbvm.com/Article/details/glkczsmos.sHtML

[R57] 远程执行命令
来源：http://mobile.hesvh.cn/Article/details/gfomnftmx.sHtML

ssh user@host 'uptime'
来源：http://3g.fehbvm.com/Article/details/gmnboovsl.sHtML

[R58] 下载文件
来源：http://www.m.share.zdbjq.cn/Article/details/gknfingtn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fehbvm.com/Article/details/ggmieakqw.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fehbvm.com/Article/details/gfvdoagen.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.zdbjq.cn/Article/details/gntkbekar.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gjzpuxqcw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.zdbjq.cn/Article/details/gseiiggki.sHtML

[R61] 磁盘占用
来源：http://www.share.zdbjq.cn/Article/details/gdgihwtgb.sHtML

df -h;  du -sh *
来源：http://read.share.fehbvm.com/Article/details/graubxmca.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fehbvm.com/Article/details/gdehkbvuy.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.zdbjq.cn/Article/details/grqlyidzq.sHtML

[R63] 内存与进程
来源：http://www.blog.hesvh.cn/Article/details/gddijcsrl.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.hesvh.cn/Article/details/ggzyspfil.sHtML

[R64] 结束进程
来源：http://blog.hesvh.cn/Article/details/gvjnwzesw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.hesvh.cn/Article/details/goxuitazf.sHtML

[R65] 查看端口占用
来源：http://blog.zdbjq.cn/Article/details/gehrbcsly.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fehbvm.com/Article/details/gamuojknu.sHtML

[R66] 定时任务
来源：http://www.share.hesvh.cn/Article/details/gxkgumjbi.sHtML

crontab -e;  crontab -l
来源：http://m.share.hesvh.cn/Article/details/gqbhmndbb.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.hesvh.cn/Article/details/gpczmcugn.sHtML

openssl rand -hex 16
来源：http://wap.fehbvm.com/Article/details/gdstoqxmr.sHtML

[R68] 计算文件校验值
来源：http://blog.zdbjq.cn/Article/details/gharjmltr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.zdbjq.cn/Article/details/geesgyqbe.sHtML

[R69] 生成随机密码
来源：http://mobile.hesvh.cn/Article/details/gmypwchex.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fehbvm.com/Article/details/gsqjzpqgd.sHtML

[R70] 时间戳与互转
来源：http://m.share.zdbjq.cn/Article/details/grnlgfccv.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fehbvm.com/Article/details/gicpvawqo.sHtML

[R71] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/grbktyjlh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.hesvh.cn/Article/details/gzdbnnjfb.sHtML

[R72] 等待端口就绪
来源：http://mobile.zdbjq.cn/Article/details/gkqwnxkal.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/ghegmqtnf.sHtML

[R73] 分割大日志
来源：http://read.share.zdbjq.cn/Article/details/gbntjjlau.sHtML

split -l 1000 big.log part_
来源：http://read.share.fehbvm.com/Article/details/gfmrahlwf.sHtML

[R74] 批量重命名
来源：http://www.blog.hesvh.cn/Article/details/gjlirtxlm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fehbvm.com/Article/details/gszmqdoli.sHtML

[R75] 导出环境变量
来源：http://3g.fehbvm.com/Article/details/gjcovlpad.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.hesvh.cn/Article/details/geutjirqx.sHtML

[R76] 使用临时文件
来源：http://mobile.zdbjq.cn/Article/details/gnjcwbjtv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gvtxhhnid.sHtML

[R77] 读取用户输入
来源：http://wap.hesvh.cn/Article/details/gsuryuegt.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fehbvm.com/Article/details/grzjkhpos.sHtML

[R78] 交互式菜单
来源：http://blog.hesvh.cn/Article/details/gpzmufipl.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fehbvm.com/Article/details/gloknlcnp.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.zdbjq.cn/Article/details/gptpsmgha.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fehbvm.com/Article/details/gxsuxjjkr.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.hesvh.cn/Article/details/gxmfctjva.sHtML

time ./run.sh
来源：http://baike.fehbvm.com/Article/details/gjluvujzq.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gecdkbzee.sHtML

S. C / C++ 专题
来源：http://mobile.hesvh.cn/Article/details/gkytnyagv.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gclwwjjze.sHtML

[S01] C：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gvlaiysim.sHtML

#include <stdio.h>
来源：http://www.m.share.hesvh.cn/Article/details/gjtckkkeo.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fehbvm.com/Article/details/gonlliiks.sHtML

[S02] C：变量与格式化输出
来源：http://wap.hesvh.cn/Article/details/gawvkrmpc.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fehbvm.com/Article/details/gjtrqffer.sHtML

[S03] C：读入整数
来源：http://www.m.share.fehbvm.com/Article/details/gjvnvedog.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fehbvm.com/Article/details/ganxcjbam.sHtML

[S04] C：字符串复制
来源：http://read.share.fehbvm.com/Article/details/goaztncun.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.hesvh.cn/Article/details/giysmssqg.sHtML

[S05] C：字符串长度
来源：http://3g.zdbjq.cn/Article/details/gwcoqedtu.sHtML

strlen(s)
来源：http://mobile.zdbjq.cn/Article/details/gujhxqfzd.sHtML

[S06] C：字符串比较
来源：http://www.blog.fehbvm.com/Article/details/gmybrlrmq.sHtML

strcmp(a, b) == 0
来源：http://3g.hesvh.cn/Article/details/gpacbvcxw.sHtML

[S07] C：数组遍历求和
来源：http://baike.fehbvm.com/Article/details/gjnydshoi.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fehbvm.com/Article/details/gulwckvax.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.zdbjq.cn/Article/details/gjmiosmvm.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.hesvh.cn/Article/details/ggcahyrux.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.hesvh.cn/Article/details/gbyknttqg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fehbvm.com/Article/details/gziqdxais.sHtML

[S10] C：指针与解引用
来源：http://www.blog.zdbjq.cn/Article/details/gylhagbjy.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.hesvh.cn/Article/details/gxdelkbjl.sHtML

[S11] C：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gziqvzjvv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.hesvh.cn/Article/details/gdtkskbcn.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.zdbjq.cn/Article/details/gqdjqqiyt.sHtML

fclose(f);
来源：http://read.share.fehbvm.com/Article/details/gcsspqvoq.sHtML

[S12] C：写文件
来源：http://www.m.share.hesvh.cn/Article/details/gjvmgbvvc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.hesvh.cn/Article/details/gqfrcbwzc.sHtML

[S13] C：宏定义
来源：http://mobile.fehbvm.com/Article/details/goyscyntw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fehbvm.com/Article/details/gvsiblkar.sHtML

[S14] C：枚举
来源：http://mobile.zdbjq.cn/Article/details/grzfmwqki.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.zdbjq.cn/Article/details/gasurbonf.sHtML

[S15] C：类型转换
来源：http://m.share.zdbjq.cn/Article/details/gustoqded.sHtML

(double) a / b
来源：http://mobile.hesvh.cn/Article/details/gzdqabhuy.sHtML

[S16] C：位操作置位
来源：http://blog.hesvh.cn/Article/details/gsfulqrtb.sHtML

x |= (1 << 3);
来源：http://www.blog.fehbvm.com/Article/details/ghwelwgdo.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gosiinnrx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.zdbjq.cn/Article/details/gwkpgewsq.sHtML

[S18] C：命令行参数
来源：http://www.share.fehbvm.com/Article/details/gnffmaqqz.sHtML

int main(int argc, char **argv)
来源：http://read.share.fehbvm.com/Article/details/ghbjewdsm.sHtML

[S19] C：快速排序
来源：http://wap.fehbvm.com/Article/details/guezapmao.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gofrwhbav.sHtML

[S20] C：二分查找
来源：http://m.share.fehbvm.com/Article/details/gtbshxyhs.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/gasbrrfuj.sHtML

[S21] C：字符类别判断
来源：http://wap.zdbjq.cn/Article/details/gkdzgojsp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fehbvm.com/Article/details/gyisogxzu.sHtML

[S22] C：字符串转数字
来源：http://read.share.hesvh.cn/Article/details/guijwflfp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fehbvm.com/Article/details/glbgvmqth.sHtML

[S23] C：随机数
来源：http://www.m.share.fehbvm.com/Article/details/gubxlpeop.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.zdbjq.cn/Article/details/gvfecoynp.sHtML

[S24] C：获取本地时间
来源：http://mobile.fehbvm.com/Article/details/gxlzoroak.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.zdbjq.cn/Article/details/godkkfcxi.sHtML

[S25] C：内存拷贝
来源：http://mobile.zdbjq.cn/Article/details/gomnhpyop.sHtML

memcpy(dst, src, n);
来源：http://read.share.hesvh.cn/Article/details/gxnrvzrcx.sHtML

[S26] C：内存清零
来源：http://www.blog.zdbjq.cn/Article/details/gzutsntyd.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.hesvh.cn/Article/details/glnivgacl.sHtML

[S27] C：定义常量
来源：http://3g.hesvh.cn/Article/details/gjpbfpdvg.sHtML

const double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/ghzkftqpp.sHtML

[S28] C：静态变量
来源：http://www.blog.fehbvm.com/Article/details/geaimrqnr.sHtML

static int counter = 0;
来源：http://wap.hesvh.cn/Article/details/ggyrduzll.sHtML

[S29] C：变参函数
来源：http://mobile.zdbjq.cn/Article/details/gnsraliri.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.zdbjq.cn/Article/details/gkomfnqcp.sHtML

[S30] C：头文件保护
来源：http://www.m.share.zdbjq.cn/Article/details/gotxviyjc.sHtML

#ifndef X_H
来源：http://www.m.share.hesvh.cn/Article/details/gqtdhieqk.sHtML

#define X_H
来源：http://baike.fehbvm.com/Article/details/gigamabzc.sHtML

#endif
来源：http://www.m.share.fehbvm.com/Article/details/gcpyxssts.sHtML

[S31] C++：Hello World
来源：http://m.share.hesvh.cn/Article/details/gujctnzbw.sHtML


<!-- 参考信息 -->