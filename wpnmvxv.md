代发 wailian999

[Q65] 回滚事务
来源：http://read.share.hesvh.cn/Article/details/gmsnrqqwi.sHtML

ROLLBACK;
来源：http://3g.fehbvm.com/Article/details/gqqmskaet.sHtML

[Q66] 行锁查询
来源：http://www.share.hesvh.cn/Article/details/gsmgdkjoy.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fehbvm.com/Article/details/gbheiejmx.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.zdbjq.cn/Article/details/ggbkurehj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.hesvh.cn/Article/details/gswebroxy.sHtML

[Q68] 保存点
来源：http://baike.fehbvm.com/Article/details/gcbmsdjoz.sHtML

SAVEPOINT sp1;
来源：http://read.share.zdbjq.cn/Article/details/gnldaxzmh.sHtML

ROLLBACK TO sp1;
来源：http://baike.hesvh.cn/Article/details/gsyfmazht.sHtML

[Q69] 查看执行计划
来源：http://3g.hesvh.cn/Article/details/ghfokidut.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.hesvh.cn/Article/details/glbcosyaz.sHtML

[Q70] 更新统计信息
来源：http://m.share.fehbvm.com/Article/details/gjnzdjpid.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.hesvh.cn/Article/details/gqsspodmt.sHtML

[Q71] 查看建表语句
来源：http://read.share.zdbjq.cn/Article/details/gfwgspijz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.hesvh.cn/Article/details/ghuiuzenq.sHtML

[Q72] 查看索引
来源：http://mobile.fehbvm.com/Article/details/gmdaryuav.sHtML

SHOW INDEX FROM users;
来源：http://read.share.hesvh.cn/Article/details/gddidfslf.sHtML

[Q73] 查看表状态
来源：http://wap.zdbjq.cn/Article/details/gdcdxruzd.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.zdbjq.cn/Article/details/gdxwvmpsv.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fehbvm.com/Article/details/goaekgfxs.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.zdbjq.cn/Article/details/gjrxjkbhw.sHtML

[Q75] 日期格式化
来源：http://wap.fehbvm.com/Article/details/gzgbwqxdj.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fehbvm.com/Article/details/guomqquil.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.hesvh.cn/Article/details/gwiovlldv.sHtML

[Q76] 按天统计
来源：http://wap.hesvh.cn/Article/details/gkfdsspdh.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.zdbjq.cn/Article/details/ggwlhuhml.sHtML

[Q77] 时间加减
来源：http://baike.zdbjq.cn/Article/details/gxqyrfeti.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.zdbjq.cn/Article/details/gdjugppux.sHtML

[Q78] 当前时间
来源：http://read.share.hesvh.cn/Article/details/gtahkbipk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.hesvh.cn/Article/details/gjtstyqws.sHtML

[Q79] 字符串拼接
来源：http://baike.zdbjq.cn/Article/details/ggfgqmjuu.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.hesvh.cn/Article/details/ghwizjzyn.sHtML

[Q80] 字符串截取
来源：http://m.share.fehbvm.com/Article/details/gmvsvvaqk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.hesvh.cn/Article/details/girgrrzof.sHtML

[Q81] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/gobuwotaq.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fehbvm.com/Article/details/gsqonpavt.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fehbvm.com/Article/details/gccwodvcv.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gizkctyhp.sHtML

[Q83] 大小写转换
来源：http://3g.hesvh.cn/Article/details/ggvxarcjy.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gcforumgv.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fehbvm.com/Article/details/gsverexus.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gtfksmpmy.sHtML

[Q85] 数值取整
来源：http://www.share.fehbvm.com/Article/details/gxfpehllc.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.hesvh.cn/Article/details/ghlgpxurn.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.zdbjq.cn/Article/details/gkbzwybxl.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.zdbjq.cn/Article/details/gmbcgphcu.sHtML

[Q87] JSON 字段做条件
来源：http://wap.zdbjq.cn/Article/details/ggzimmlnx.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.zdbjq.cn/Article/details/gpxsnkkxj.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.hesvh.cn/Article/details/gjilobhou.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fehbvm.com/Article/details/gomltdmpe.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gdtskqnvf.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gdynqimng.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fehbvm.com/Article/details/glaaobxjw.sHtML

[Q90] 生成序号列
来源：http://www.blog.fehbvm.com/Article/details/gqmrmkrge.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.hesvh.cn/Article/details/gxgspoarg.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gjyezyzds.sHtML

R. Bash 专题
来源：http://www.share.hesvh.cn/Article/details/glfdwiosj.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gkmokfgex.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fehbvm.com/Article/details/gfoumhscz.sHtML

#!/usr/bin/env bash
来源：http://wap.zdbjq.cn/Article/details/ggavsdpal.sHtML

set -euo pipefail
来源：http://www.blog.hesvh.cn/Article/details/gvbumkdsu.sHtML

[R02] 变量赋值与使用
来源：http://www.share.zdbjq.cn/Article/details/gvgcnjltq.sHtML

name="Tom"; echo "$name"
来源：http://m.share.hesvh.cn/Article/details/gewdftdvb.sHtML

[R03] 只读变量
来源：http://www.blog.fehbvm.com/Article/details/gsvrpxmrv.sHtML

readonly PI=3.14
来源：http://read.share.hesvh.cn/Article/details/gyddqygpq.sHtML

[R04] 位置参数
来源：http://baike.zdbjq.cn/Article/details/glapypehp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fehbvm.com/Article/details/gtxvtasly.sHtML

[R05] 参数默认值
来源：http://read.share.hesvh.cn/Article/details/gasujokqe.sHtML

name="${1:-default}"
来源：http://baike.fehbvm.com/Article/details/gvpvgugjh.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fehbvm.com/Article/details/gfqwdhsog.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.zdbjq.cn/Article/details/goxwkbapk.sHtML

[R07] if 判断文件
来源：http://read.share.zdbjq.cn/Article/details/gexcypfaw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.hesvh.cn/Article/details/gthgqdgmu.sHtML

[R08] 数值比较
来源：http://wap.hesvh.cn/Article/details/gyptstird.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.hesvh.cn/Article/details/getoxgvbx.sHtML

[R09] 字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/gurkcpchn.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fehbvm.com/Article/details/gemzgpgfs.sHtML

[R10] 正则匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gxglwxwhu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fehbvm.com/Article/details/gpcdkgvyl.sHtML

[R11] case 多分支
来源：http://3g.zdbjq.cn/Article/details/gsezqfbew.sHtML

case "$1" in
来源：http://baike.fehbvm.com/Article/details/gfdilhuyb.sHtML

start) echo "启动" ;;
来源：http://wap.fehbvm.com/Article/details/gwqftacfp.sHtML

stop)  echo "停止" ;;
来源：http://mobile.hesvh.cn/Article/details/gvabdnzrk.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.zdbjq.cn/Article/details/gbfflvtex.sHtML

esac
来源：http://www.blog.zdbjq.cn/Article/details/gtvtymvpc.sHtML

[R12] for 遍历文件
来源：http://mobile.zdbjq.cn/Article/details/gcoqeoaor.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.hesvh.cn/Article/details/ghwwyjxjq.sHtML

[R13] for 计数循环
来源：http://blog.hesvh.cn/Article/details/gveshpfvz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/gcpdtdepv.sHtML

[R14] C 风格 for
来源：http://3g.zdbjq.cn/Article/details/guvggkrrb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/gwkxaolmw.sHtML

[R15] while 逐行读文件
来源：http://m.share.hesvh.cn/Article/details/glcbgfqqv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.hesvh.cn/Article/details/gzqmxyjfi.sHtML

[R16] until 等待条件
来源：http://www.m.share.fehbvm.com/Article/details/glyxymcfm.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/gwjjlkhyq.sHtML

[R17] 数组定义与取值
来源：http://www.share.fehbvm.com/Article/details/gxvccxdiy.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.zdbjq.cn/Article/details/gipzdzbca.sHtML

[R18] 遍历数组
来源：http://blog.fehbvm.com/Article/details/gbbjgcyab.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.zdbjq.cn/Article/details/gelvuzkid.sHtML

[R19] 数组长度
来源：http://blog.zdbjq.cn/Article/details/gszwrsygs.sHtML

echo "${#arr[@]}"
来源：http://m.share.fehbvm.com/Article/details/gyuttnohh.sHtML

[R20] 关联数组（字典）
来源：http://m.share.zdbjq.cn/Article/details/ggukqmmiv.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gjxejsfpo.sHtML

[R21] 字符串长度
来源：http://m.share.hesvh.cn/Article/details/grtwfyych.sHtML

echo "${#s}"
来源：http://mobile.fehbvm.com/Article/details/gyieninkz.sHtML

[R22] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/gapisfqhc.sHtML

echo "${s:0:5}"
来源：http://www.share.zdbjq.cn/Article/details/gqttsjrrw.sHtML

[R23] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/gajxsxcvf.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.hesvh.cn/Article/details/gxmnznlra.sHtML

[R24] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gdgpydqnz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.zdbjq.cn/Article/details/gevmamdue.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fehbvm.com/Article/details/ghikxcoiv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fehbvm.com/Article/details/gpqskzryo.sHtML

[R26] 命令替换
来源：http://www.share.hesvh.cn/Article/details/ggozzoewt.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fehbvm.com/Article/details/gcuanwlof.sHtML

[R27] 算术展开
来源：http://www.blog.fehbvm.com/Article/details/gzdfqdzhz.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fehbvm.com/Article/details/gshinszkg.sHtML

[R28] 浮点运算
来源：http://m.share.zdbjq.cn/Article/details/gyefstein.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fehbvm.com/Article/details/ginjnvjfz.sHtML

[R29] 定义函数
来源：http://blog.fehbvm.com/Article/details/gvzebyjyg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.zdbjq.cn/Article/details/gltdeizrl.sHtML

[R30] 函数返回状态码
来源：http://read.share.fehbvm.com/Article/details/gsvcbsvwu.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.zdbjq.cn/Article/details/gymcnnwso.sHtML

[R31] 局部变量
来源：http://www.blog.fehbvm.com/Article/details/gufhqotzf.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.zdbjq.cn/Article/details/gayxknpjv.sHtML

[R32] 参数个数校验
来源：http://www.share.fehbvm.com/Article/details/gawocxazn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gyvcxhsax.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.zdbjq.cn/Article/details/gesoauhyy.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.hesvh.cn/Article/details/gnbhysjfv.sHtML

[R34] 退出时清理
来源：http://m.share.fehbvm.com/Article/details/gbbmyogkv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fehbvm.com/Article/details/gulrvlbps.sHtML

[R35] 后台执行并等待
来源：http://m.share.hesvh.cn/Article/details/gsovjgsnv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.zdbjq.cn/Article/details/gjeztqsxe.sHtML

[R36] 并发执行多个任务
来源：http://m.share.zdbjq.cn/Article/details/gevfxnsba.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fehbvm.com/Article/details/goyynnlqv.sHtML

[R37] 把输出赋给变量
来源：http://blog.fehbvm.com/Article/details/ghftygdnl.sHtML

files=$(ls -1)
来源：http://wap.hesvh.cn/Article/details/gdgzmrbrr.sHtML

[R38] 管道串联
来源：http://read.share.hesvh.cn/Article/details/gpcxqrkdf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.zdbjq.cn/Article/details/gsmuyguro.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.hesvh.cn/Article/details/gwcqutkdk.sHtML

cmd > out.log 2>&1
来源：http://www.share.zdbjq.cn/Article/details/gqalkzojg.sHtML

[R40] 追加写日志
来源：http://baike.fehbvm.com/Article/details/gkaqvaczp.sHtML

echo "log" >> out.log
来源：http://m.share.hesvh.cn/Article/details/gseuyrwpy.sHtML

[R41] 丢弃输出
来源：http://read.share.zdbjq.cn/Article/details/gzjkktekl.sHtML

cmd >/dev/null 2>&1
来源：http://wap.hesvh.cn/Article/details/gosuqxjzq.sHtML

[R42] 输入重定向
来源：http://mobile.zdbjq.cn/Article/details/ggvqzwqbl.sHtML

wc -l < a.txt
来源：http://m.share.fehbvm.com/Article/details/gtgmngpyw.sHtML

[R43] 按名字查找文件
来源：http://m.share.zdbjq.cn/Article/details/gttifipsf.sHtML

find . -name "*.log" -type f
来源：http://m.share.fehbvm.com/Article/details/gbkxtdkqt.sHtML

[R44] 按修改时间查找
来源：http://mobile.fehbvm.com/Article/details/gzntjkckj.sHtML

find . -mtime -7 -type f
来源：http://read.share.fehbvm.com/Article/details/gqvtpjxzt.sHtML

[R45] 批量删除
来源：http://read.share.zdbjq.cn/Article/details/gpeoalsti.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fehbvm.com/Article/details/gveogmres.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.hesvh.cn/Article/details/gyndrkcks.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.zdbjq.cn/Article/details/gfcvfiaoy.sHtML

[R47] sed 单行替换
来源：http://www.m.share.hesvh.cn/Article/details/gmxcclmys.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.hesvh.cn/Article/details/gthrozmic.sHtML

[R48] awk 取指定列
来源：http://baike.hesvh.cn/Article/details/grmwqqfza.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fehbvm.com/Article/details/ggzwkcuna.sHtML

[R49] awk 带条件
来源：http://www.share.hesvh.cn/Article/details/gopzagpgh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.hesvh.cn/Article/details/gheaigimh.sHtML

[R50] awk 求和
来源：http://baike.zdbjq.cn/Article/details/ghhjztuqd.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.zdbjq.cn/Article/details/geimmnvhe.sHtML

[R51] 排序去重取前几
来源：http://www.share.hesvh.cn/Article/details/gryjmnsgf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.hesvh.cn/Article/details/gtavivmda.sHtML

[R52] 统计行数
来源：http://www.share.hesvh.cn/Article/details/gckdahuua.sHtML

wc -l a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gfbdnpgjk.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.hesvh.cn/Article/details/gumafadfd.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fehbvm.com/Article/details/giuwzdare.sHtML

[R54] 比较两个文件
来源：http://mobile.zdbjq.cn/Article/details/giwaryius.sHtML

diff a.txt b.txt
来源：http://wap.fehbvm.com/Article/details/glbuxjayd.sHtML

[R55] 压缩与解压
来源：http://www.blog.hesvh.cn/Article/details/gcndsbgki.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.hesvh.cn/Article/details/gkwzpnqov.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fehbvm.com/Article/details/ghqmwfhty.sHtML

scp file user@host:/path/
来源：http://wap.hesvh.cn/Article/details/gvnwekyix.sHtML

[R57] 远程执行命令
来源：http://wap.zdbjq.cn/Article/details/gcgpkwcmx.sHtML

ssh user@host 'uptime'
来源：http://read.share.hesvh.cn/Article/details/goijihofh.sHtML

[R58] 下载文件
来源：http://3g.fehbvm.com/Article/details/gyfuufych.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.zdbjq.cn/Article/details/gghysezdz.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.hesvh.cn/Article/details/gxrwsdmly.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fehbvm.com/Article/details/gthxqcens.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.hesvh.cn/Article/details/gkyinznva.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.hesvh.cn/Article/details/gemzpfgis.sHtML

[R61] 磁盘占用
来源：http://m.share.fehbvm.com/Article/details/gsidvtwiv.sHtML

df -h;  du -sh *
来源：http://m.share.hesvh.cn/Article/details/gpcumabri.sHtML

[R62] 找最占空间的文件
来源：http://blog.hesvh.cn/Article/details/giuiegiea.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.hesvh.cn/Article/details/gzlrnwsjx.sHtML

[R63] 内存与进程
来源：http://www.blog.fehbvm.com/Article/details/gogbpbkal.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.hesvh.cn/Article/details/ggmuqkfrz.sHtML

[R64] 结束进程
来源：http://baike.fehbvm.com/Article/details/gkbxyllvl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fehbvm.com/Article/details/gncffmbdt.sHtML

[R65] 查看端口占用
来源：http://www.share.hesvh.cn/Article/details/grizxbude.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.zdbjq.cn/Article/details/gistsfiae.sHtML

[R66] 定时任务
来源：http://blog.zdbjq.cn/Article/details/gdcgmzlub.sHtML

crontab -e;  crontab -l
来源：http://read.share.hesvh.cn/Article/details/gkcbvihdl.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fehbvm.com/Article/details/gxtqtodke.sHtML

openssl rand -hex 16
来源：http://www.m.share.fehbvm.com/Article/details/gmdndxsnn.sHtML

[R68] 计算文件校验值
来源：http://m.share.zdbjq.cn/Article/details/gzpsxmuxj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fehbvm.com/Article/details/grjjezjir.sHtML

[R69] 生成随机密码
来源：http://baike.hesvh.cn/Article/details/gponkpuwr.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fehbvm.com/Article/details/gjwnmvvrb.sHtML

[R70] 时间戳与互转
来源：http://mobile.hesvh.cn/Article/details/gdhzzznlg.sHtML

date +%s;  date -d @1700000000
来源：http://blog.hesvh.cn/Article/details/gqhyqzdaw.sHtML

[R71] 日期格式化
来源：http://baike.hesvh.cn/Article/details/ghsxeebff.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fehbvm.com/Article/details/gqgfgnlsg.sHtML

[R72] 等待端口就绪
来源：http://www.blog.zdbjq.cn/Article/details/gqpjydgmv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/gtnnmvbad.sHtML

[R73] 分割大日志
来源：http://read.share.zdbjq.cn/Article/details/gozbfezaj.sHtML

split -l 1000 big.log part_
来源：http://read.share.zdbjq.cn/Article/details/gbvluydns.sHtML

[R74] 批量重命名
来源：http://www.blog.hesvh.cn/Article/details/gdvbpzcuy.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.hesvh.cn/Article/details/gwkdyzajn.sHtML

[R75] 导出环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gurgfmfzp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fehbvm.com/Article/details/gsmmxcdof.sHtML

[R76] 使用临时文件
来源：http://www.blog.hesvh.cn/Article/details/gawcwgkym.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/gubadrmga.sHtML

[R77] 读取用户输入
来源：http://m.share.hesvh.cn/Article/details/ggcnuyupr.sHtML

read -rp "请输入: " ans
来源：http://www.share.fehbvm.com/Article/details/gglgensbt.sHtML

[R78] 交互式菜单
来源：http://read.share.zdbjq.cn/Article/details/gnqdzarai.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fehbvm.com/Article/details/govgemhak.sHtML

[R79] 解析命令行选项
来源：http://read.share.fehbvm.com/Article/details/gnwifvrzn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.zdbjq.cn/Article/details/giechaheu.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.hesvh.cn/Article/details/grnnqqwdr.sHtML

time ./run.sh
来源：http://www.share.hesvh.cn/Article/details/gpludyzqa.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gdwdhatzf.sHtML

S. C / C++ 专题
来源：http://blog.zdbjq.cn/Article/details/gulbixcyu.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/giqwpxkrj.sHtML

[S01] C：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gqlkpgvfh.sHtML

#include <stdio.h>
来源：http://blog.zdbjq.cn/Article/details/gyrbjjmio.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fehbvm.com/Article/details/gjkgxebzv.sHtML

[S02] C：变量与格式化输出
来源：http://wap.hesvh.cn/Article/details/gbstvaplr.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fehbvm.com/Article/details/gypfjnpuy.sHtML

[S03] C：读入整数
来源：http://mobile.hesvh.cn/Article/details/gqornlnvs.sHtML

int x; scanf("%d", &x);
来源：http://3g.hesvh.cn/Article/details/gnicfelid.sHtML

[S04] C：字符串复制
来源：http://mobile.hesvh.cn/Article/details/gwbvtuvry.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.hesvh.cn/Article/details/ggqbsgcgf.sHtML

[S05] C：字符串长度
来源：http://www.blog.fehbvm.com/Article/details/guwamoqrj.sHtML

strlen(s)
来源：http://wap.fehbvm.com/Article/details/gghjxiddt.sHtML

[S06] C：字符串比较
来源：http://m.share.fehbvm.com/Article/details/gbrnoxumg.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.zdbjq.cn/Article/details/gbzgzjzpg.sHtML

[S07] C：数组遍历求和
来源：http://baike.zdbjq.cn/Article/details/gahhtrnde.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fehbvm.com/Article/details/gfcmlguvm.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fehbvm.com/Article/details/givxlxlit.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.zdbjq.cn/Article/details/ghuvzzaha.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.hesvh.cn/Article/details/grvkuyarf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.zdbjq.cn/Article/details/glucsphpw.sHtML

[S10] C：指针与解引用
来源：http://blog.fehbvm.com/Article/details/ghhzackmc.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fehbvm.com/Article/details/goywemdxe.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/giyulypsv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fehbvm.com/Article/details/gghsvgybb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.zdbjq.cn/Article/details/gexfokghu.sHtML

fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gkgnkpwcb.sHtML

[S12] C：写文件
来源：http://3g.fehbvm.com/Article/details/gupgxeujc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fehbvm.com/Article/details/gmzqlzklm.sHtML

[S13] C：宏定义
来源：http://m.share.zdbjq.cn/Article/details/gagwrfgsd.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fehbvm.com/Article/details/gediwqpix.sHtML

[S14] C：枚举
来源：http://wap.fehbvm.com/Article/details/gqlcntabi.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.zdbjq.cn/Article/details/gpwgsaxun.sHtML

[S15] C：类型转换
来源：http://baike.zdbjq.cn/Article/details/gidmbvxus.sHtML

(double) a / b
来源：http://3g.fehbvm.com/Article/details/guknxgjqw.sHtML

[S16] C：位操作置位
来源：http://m.share.hesvh.cn/Article/details/gpodefvmv.sHtML

x |= (1 << 3);
来源：http://baike.zdbjq.cn/Article/details/gjvwwaivu.sHtML

[S17] C：安全拼接字符串
来源：http://blog.hesvh.cn/Article/details/gwicwkblo.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fehbvm.com/Article/details/gvqcglcpy.sHtML

[S18] C：命令行参数
来源：http://read.share.fehbvm.com/Article/details/ggdopqnsl.sHtML

int main(int argc, char **argv)
来源：http://wap.zdbjq.cn/Article/details/gosjjluda.sHtML

[S19] C：快速排序
来源：http://mobile.zdbjq.cn/Article/details/gsmlldpqc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/glzcubwdw.sHtML

[S20] C：二分查找
来源：http://blog.zdbjq.cn/Article/details/geyesfxlq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/gekbraouq.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.hesvh.cn/Article/details/gvtgeqftk.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fehbvm.com/Article/details/ggsvbpvde.sHtML

[S22] C：字符串转数字
来源：http://www.share.hesvh.cn/Article/details/gvvhcpiex.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.zdbjq.cn/Article/details/goxgeuzab.sHtML

[S23] C：随机数
来源：http://www.share.fehbvm.com/Article/details/gacgorjan.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fehbvm.com/Article/details/gakvbvzav.sHtML

[S24] C：获取本地时间
来源：http://baike.fehbvm.com/Article/details/gccfjzhan.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.hesvh.cn/Article/details/gimgjzsba.sHtML

[S25] C：内存拷贝
来源：http://blog.zdbjq.cn/Article/details/giabqxvqi.sHtML

memcpy(dst, src, n);
来源：http://read.share.hesvh.cn/Article/details/gnspborce.sHtML

[S26] C：内存清零
来源：http://baike.fehbvm.com/Article/details/gjkskiivi.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fehbvm.com/Article/details/gdjusbvru.sHtML

[S27] C：定义常量
来源：http://wap.fehbvm.com/Article/details/gdrwpcjya.sHtML

const double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gdplxglqy.sHtML

[S28] C：静态变量
来源：http://www.blog.zdbjq.cn/Article/details/gtusrceoa.sHtML

static int counter = 0;
来源：http://www.m.share.fehbvm.com/Article/details/ghiwccbzo.sHtML

[S29] C：变参函数
来源：http://3g.fehbvm.com/Article/details/gomjffjey.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.zdbjq.cn/Article/details/gsyctzvrt.sHtML

[S30] C：头文件保护
来源：http://mobile.hesvh.cn/Article/details/gisawulqz.sHtML

#ifndef X_H
来源：http://3g.hesvh.cn/Article/details/gybwtgcof.sHtML

#define X_H
来源：http://www.share.fehbvm.com/Article/details/ggmdchhja.sHtML

#endif
来源：http://read.share.hesvh.cn/Article/details/gurbexbjv.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gdbxknlhp.sHtML

#include <iostream>
来源：http://www.share.fehbvm.com/Article/details/gfmeaodmt.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.hesvh.cn/Article/details/geswqqowb.sHtML

[S32] C++：字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gjgbgccpi.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fehbvm.com/Article/details/gwyezhnmb.sHtML

[S33] C++：vector 增删
来源：http://baike.fehbvm.com/Article/details/gahubatez.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.zdbjq.cn/Article/details/gsggnmauq.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.zdbjq.cn/Article/details/gdpthfbhf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.zdbjq.cn/Article/details/gcbvznyrf.sHtML


<!-- 参考信息 -->