代发 wailian999

ROLLBACK TO sp1;
来源：http://blog.fehbvm.com/Article/details/guyynqrpm.sHtML

[Q69] 查看执行计划
来源：http://3g.fehbvm.com/Article/details/gdtmjlzih.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fehbvm.com/Article/details/gvqwrawki.sHtML

[Q70] 更新统计信息
来源：http://m.share.hesvh.cn/Article/details/ghafkffjs.sHtML

ANALYZE TABLE users;
来源：http://m.share.fehbvm.com/Article/details/gczqnfbrk.sHtML

[Q71] 查看建表语句
来源：http://3g.fehbvm.com/Article/details/gxhshrpxw.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.hesvh.cn/Article/details/gvalgpnuw.sHtML

[Q72] 查看索引
来源：http://www.share.zdbjq.cn/Article/details/giioevmih.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fehbvm.com/Article/details/gyusrfyim.sHtML

[Q73] 查看表状态
来源：http://read.share.zdbjq.cn/Article/details/ggnbynzxb.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.hesvh.cn/Article/details/glafpbjtd.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fehbvm.com/Article/details/grdxgdfqd.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.zdbjq.cn/Article/details/gtsiysmml.sHtML

[Q75] 日期格式化
来源：http://3g.fehbvm.com/Article/details/gamahvwsz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gzgymkysc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.zdbjq.cn/Article/details/ggkqicevj.sHtML

[Q76] 按天统计
来源：http://read.share.hesvh.cn/Article/details/gkckhrnag.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.zdbjq.cn/Article/details/gryehpsbe.sHtML

[Q77] 时间加减
来源：http://www.m.share.fehbvm.com/Article/details/grwqcnmea.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.zdbjq.cn/Article/details/ggibodhzx.sHtML

[Q78] 当前时间
来源：http://www.m.share.hesvh.cn/Article/details/gsuhblcnv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.hesvh.cn/Article/details/gwwvrsydq.sHtML

[Q79] 字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/gurhohaoz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fehbvm.com/Article/details/glbpjheis.sHtML

[Q80] 字符串截取
来源：http://3g.hesvh.cn/Article/details/gfqrfawsr.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/ggvzuiepf.sHtML

[Q81] 字符串替换
来源：http://baike.hesvh.cn/Article/details/gfllgljec.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fehbvm.com/Article/details/gidzkgbhg.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.zdbjq.cn/Article/details/guxnfwkre.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gwctsfmme.sHtML

[Q83] 大小写转换
来源：http://wap.hesvh.cn/Article/details/gwulucouk.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gqajwbnry.sHtML

[Q84] 去除首尾空格
来源：http://baike.zdbjq.cn/Article/details/gnvwmayyu.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/guvrmtepx.sHtML

[Q85] 数值取整
来源：http://wap.fehbvm.com/Article/details/gqhkrjzpl.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.hesvh.cn/Article/details/gvgqlbcjj.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.hesvh.cn/Article/details/grovbbarb.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.zdbjq.cn/Article/details/gfcrqconc.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.hesvh.cn/Article/details/gshjizjhu.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.hesvh.cn/Article/details/gasneitqe.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.zdbjq.cn/Article/details/gdsawjuwo.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.zdbjq.cn/Article/details/gcfypxydg.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gbbwwfdds.sHtML

[Q89] 判断表是否存在
来源：http://blog.fehbvm.com/Article/details/gagahybnr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.hesvh.cn/Article/details/gkcxxfuez.sHtML

[Q90] 生成序号列
来源：http://3g.fehbvm.com/Article/details/gjroqotbp.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fehbvm.com/Article/details/gmyhapdbp.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gckhntetr.sHtML

R. Bash 专题
来源：http://www.blog.zdbjq.cn/Article/details/gtfrwtxne.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gldjzopsg.sHtML

[R01] shebang 与严格模式
来源：http://mobile.zdbjq.cn/Article/details/ggfdsutow.sHtML

#!/usr/bin/env bash
来源：http://3g.zdbjq.cn/Article/details/genjpskpg.sHtML

set -euo pipefail
来源：http://m.share.fehbvm.com/Article/details/giowmgxps.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fehbvm.com/Article/details/gyrpdefxa.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.zdbjq.cn/Article/details/gfgezepoy.sHtML

[R03] 只读变量
来源：http://baike.fehbvm.com/Article/details/grtktblvp.sHtML

readonly PI=3.14
来源：http://wap.fehbvm.com/Article/details/gtimodcij.sHtML

[R04] 位置参数
来源：http://www.m.share.fehbvm.com/Article/details/gjzgktfmv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fehbvm.com/Article/details/gpyostkma.sHtML

[R05] 参数默认值
来源：http://m.share.hesvh.cn/Article/details/gfzmlycxz.sHtML

name="${1:-default}"
来源：http://baike.zdbjq.cn/Article/details/gjwnilegr.sHtML

[R06] 判断命令是否存在
来源：http://wap.hesvh.cn/Article/details/galwyxrnz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gxmkwgolo.sHtML

[R07] if 判断文件
来源：http://www.blog.zdbjq.cn/Article/details/gdyzuyojl.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gnpgrqgts.sHtML

[R08] 数值比较
来源：http://3g.fehbvm.com/Article/details/gdkkwqtac.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.hesvh.cn/Article/details/gjezehnfl.sHtML

[R09] 字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gjazaabnt.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.hesvh.cn/Article/details/gzhfmonje.sHtML

[R10] 正则匹配
来源：http://baike.fehbvm.com/Article/details/gkyplrwsg.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fehbvm.com/Article/details/gvfbdidak.sHtML

[R11] case 多分支
来源：http://wap.hesvh.cn/Article/details/gtzjsvwps.sHtML

case "$1" in
来源：http://www.share.hesvh.cn/Article/details/gtyucmwtk.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gscouwmzh.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fehbvm.com/Article/details/ggxujrzwu.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gnztrrtlv.sHtML

esac
来源：http://www.m.share.fehbvm.com/Article/details/gbzcvtlos.sHtML

[R12] for 遍历文件
来源：http://www.share.fehbvm.com/Article/details/gwhipgjlq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.zdbjq.cn/Article/details/gewxoxmrx.sHtML

[R13] for 计数循环
来源：http://read.share.hesvh.cn/Article/details/gxisdlcat.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/glkwbhhlx.sHtML

[R14] C 风格 for
来源：http://www.m.share.zdbjq.cn/Article/details/gvdfkrrqt.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/gbshmfzpu.sHtML

[R15] while 逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gfkoarwdc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fehbvm.com/Article/details/gnsjwhpub.sHtML

[R16] until 等待条件
来源：http://read.share.hesvh.cn/Article/details/gccflrxrm.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/gkrziwgnv.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.hesvh.cn/Article/details/goigpfcnh.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fehbvm.com/Article/details/gfwyibkow.sHtML

[R18] 遍历数组
来源：http://wap.zdbjq.cn/Article/details/gmpsgunlu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fehbvm.com/Article/details/gscbpgoij.sHtML

[R19] 数组长度
来源：http://mobile.hesvh.cn/Article/details/gvqofbvje.sHtML

echo "${#arr[@]}"
来源：http://baike.fehbvm.com/Article/details/gwnfcsbjg.sHtML

[R20] 关联数组（字典）
来源：http://www.share.hesvh.cn/Article/details/gobazlotr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fehbvm.com/Article/details/gpvebprvp.sHtML

[R21] 字符串长度
来源：http://www.share.hesvh.cn/Article/details/gzpriyevs.sHtML

echo "${#s}"
来源：http://wap.zdbjq.cn/Article/details/girjnnfvp.sHtML

[R22] 截取子串
来源：http://www.share.fehbvm.com/Article/details/gpanpakky.sHtML

echo "${s:0:5}"
来源：http://blog.fehbvm.com/Article/details/glxfniulb.sHtML

[R23] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gtoggymzn.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.hesvh.cn/Article/details/goekcpjis.sHtML

[R24] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/gmcxdoamh.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fehbvm.com/Article/details/gbouixaiv.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.hesvh.cn/Article/details/glcfbcnpu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.zdbjq.cn/Article/details/gkhloriky.sHtML

[R26] 命令替换
来源：http://read.share.fehbvm.com/Article/details/gtsuqoepr.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.hesvh.cn/Article/details/goiypypxj.sHtML

[R27] 算术展开
来源：http://www.m.share.fehbvm.com/Article/details/genugzmhr.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fehbvm.com/Article/details/gaoqubndq.sHtML

[R28] 浮点运算
来源：http://m.share.zdbjq.cn/Article/details/gkmzgflun.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.hesvh.cn/Article/details/gzvwsaamd.sHtML

[R29] 定义函数
来源：http://mobile.hesvh.cn/Article/details/gjehixyab.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.hesvh.cn/Article/details/gbjxnjudx.sHtML

[R30] 函数返回状态码
来源：http://www.share.zdbjq.cn/Article/details/gutjfxxkl.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.zdbjq.cn/Article/details/gslazolzv.sHtML

[R31] 局部变量
来源：http://www.blog.fehbvm.com/Article/details/gmqxckqjz.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fehbvm.com/Article/details/gnrkwhodd.sHtML

[R32] 参数个数校验
来源：http://www.blog.fehbvm.com/Article/details/gpxtdxgkb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/gtspahfif.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.zdbjq.cn/Article/details/gspjekfuk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.hesvh.cn/Article/details/glsqwqrdw.sHtML

[R34] 退出时清理
来源：http://mobile.hesvh.cn/Article/details/gauwaufij.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fehbvm.com/Article/details/gkwxlwxnp.sHtML

[R35] 后台执行并等待
来源：http://wap.fehbvm.com/Article/details/glrwrdqzy.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fehbvm.com/Article/details/gcxwsyjes.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fehbvm.com/Article/details/gqpsfhvgn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fehbvm.com/Article/details/gytynnfuk.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fehbvm.com/Article/details/gyzucszhs.sHtML

files=$(ls -1)
来源：http://3g.hesvh.cn/Article/details/gecnvubcl.sHtML

[R38] 管道串联
来源：http://3g.hesvh.cn/Article/details/gzcznezvm.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fehbvm.com/Article/details/ggdqxdvdw.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.zdbjq.cn/Article/details/gxlooysvl.sHtML

cmd > out.log 2>&1
来源：http://wap.hesvh.cn/Article/details/gqherauob.sHtML

[R40] 追加写日志
来源：http://baike.hesvh.cn/Article/details/gmegpngxi.sHtML

echo "log" >> out.log
来源：http://baike.fehbvm.com/Article/details/gfzhmjafj.sHtML

[R41] 丢弃输出
来源：http://mobile.fehbvm.com/Article/details/gbwjyrdmh.sHtML

cmd >/dev/null 2>&1
来源：http://wap.zdbjq.cn/Article/details/gpnqgaodx.sHtML

[R42] 输入重定向
来源：http://read.share.hesvh.cn/Article/details/gsobboyso.sHtML

wc -l < a.txt
来源：http://3g.fehbvm.com/Article/details/glmvunaeo.sHtML

[R43] 按名字查找文件
来源：http://blog.hesvh.cn/Article/details/gtihiejze.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.hesvh.cn/Article/details/gzuorcysa.sHtML

[R44] 按修改时间查找
来源：http://baike.zdbjq.cn/Article/details/gyhlernbv.sHtML

find . -mtime -7 -type f
来源：http://blog.zdbjq.cn/Article/details/gqhkydvqx.sHtML

[R45] 批量删除
来源：http://read.share.hesvh.cn/Article/details/gqbyqprxh.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.zdbjq.cn/Article/details/gknzrngzd.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.hesvh.cn/Article/details/giqpvvama.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.zdbjq.cn/Article/details/gwqczhtly.sHtML

[R47] sed 单行替换
来源：http://blog.fehbvm.com/Article/details/gazyriiof.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gucrfsdsw.sHtML

[R48] awk 取指定列
来源：http://www.blog.hesvh.cn/Article/details/gpwujxhbk.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gseumdsai.sHtML

[R49] awk 带条件
来源：http://wap.zdbjq.cn/Article/details/gubuizlxq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.hesvh.cn/Article/details/gyqlvmvbv.sHtML

[R50] awk 求和
来源：http://www.blog.fehbvm.com/Article/details/gcjgnptoa.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fehbvm.com/Article/details/gowzdqrlw.sHtML

[R51] 排序去重取前几
来源：http://read.share.hesvh.cn/Article/details/gykwcebmb.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.hesvh.cn/Article/details/gjmfesvmp.sHtML

[R52] 统计行数
来源：http://read.share.fehbvm.com/Article/details/gprdhxmoj.sHtML

wc -l a.txt
来源：http://mobile.fehbvm.com/Article/details/gojfhhgdg.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fehbvm.com/Article/details/gnilahvcb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.zdbjq.cn/Article/details/gcfrxlugb.sHtML

[R54] 比较两个文件
来源：http://read.share.hesvh.cn/Article/details/ggunkdydk.sHtML

diff a.txt b.txt
来源：http://3g.fehbvm.com/Article/details/gcuxcpigh.sHtML

[R55] 压缩与解压
来源：http://www.blog.fehbvm.com/Article/details/gwriufpyw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fehbvm.com/Article/details/gbangiuto.sHtML

[R56] 远程拷贝
来源：http://mobile.fehbvm.com/Article/details/gnfcjqtzh.sHtML

scp file user@host:/path/
来源：http://www.blog.hesvh.cn/Article/details/gjcozoepb.sHtML

[R57] 远程执行命令
来源：http://www.blog.hesvh.cn/Article/details/gfbpsvrvw.sHtML

ssh user@host 'uptime'
来源：http://m.share.fehbvm.com/Article/details/gwlaekjcp.sHtML

[R58] 下载文件
来源：http://www.share.hesvh.cn/Article/details/gugvqnexb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.hesvh.cn/Article/details/gbdjmxtij.sHtML

[R59] 发 POST JSON
来源：http://blog.fehbvm.com/Article/details/gcolnfyaw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.hesvh.cn/Article/details/gvsdtnfnx.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.zdbjq.cn/Article/details/ghokayucp.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.zdbjq.cn/Article/details/gskxohjih.sHtML

[R61] 磁盘占用
来源：http://blog.fehbvm.com/Article/details/gsfgohhni.sHtML

df -h;  du -sh *
来源：http://baike.hesvh.cn/Article/details/glhvcpsvk.sHtML

[R62] 找最占空间的文件
来源：http://m.share.zdbjq.cn/Article/details/geznloign.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fehbvm.com/Article/details/gqccvmojz.sHtML

[R63] 内存与进程
来源：http://mobile.hesvh.cn/Article/details/gofshnbgf.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.zdbjq.cn/Article/details/gzqfmlehn.sHtML

[R64] 结束进程
来源：http://m.share.hesvh.cn/Article/details/gaspvijov.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fehbvm.com/Article/details/gfqlevxqp.sHtML

[R65] 查看端口占用
来源：http://www.blog.zdbjq.cn/Article/details/gejhrqwgx.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.hesvh.cn/Article/details/gwuzawgvw.sHtML

[R66] 定时任务
来源：http://m.share.zdbjq.cn/Article/details/gkqeckrmv.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fehbvm.com/Article/details/gxhmicwpn.sHtML

[R67] 生成随机十六进制串
来源：http://3g.hesvh.cn/Article/details/geeenpprr.sHtML

openssl rand -hex 16
来源：http://mobile.hesvh.cn/Article/details/ghfgykirz.sHtML

[R68] 计算文件校验值
来源：http://mobile.hesvh.cn/Article/details/gfudfxzjh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.hesvh.cn/Article/details/gtbstwkiv.sHtML

[R69] 生成随机密码
来源：http://blog.hesvh.cn/Article/details/guksrlepe.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.zdbjq.cn/Article/details/gcxhhtwyk.sHtML

[R70] 时间戳与互转
来源：http://read.share.hesvh.cn/Article/details/gkllffrcu.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.hesvh.cn/Article/details/gmimgcaea.sHtML

[R71] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/ggzifjbuc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.hesvh.cn/Article/details/gpgwosqwl.sHtML

[R72] 等待端口就绪
来源：http://www.share.hesvh.cn/Article/details/gaycugebb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gglcfauhg.sHtML

[R73] 分割大日志
来源：http://3g.hesvh.cn/Article/details/gjpeszpui.sHtML

split -l 1000 big.log part_
来源：http://read.share.fehbvm.com/Article/details/gabacakgh.sHtML

[R74] 批量重命名
来源：http://3g.zdbjq.cn/Article/details/glwflidzx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.hesvh.cn/Article/details/glzkgjggs.sHtML

[R75] 导出环境变量
来源：http://m.share.hesvh.cn/Article/details/gieuidivt.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.hesvh.cn/Article/details/gkfphrozr.sHtML

[R76] 使用临时文件
来源：http://blog.zdbjq.cn/Article/details/guaindpyj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/glfspexbl.sHtML

[R77] 读取用户输入
来源：http://www.blog.fehbvm.com/Article/details/grpvgzhgn.sHtML

read -rp "请输入: " ans
来源：http://wap.zdbjq.cn/Article/details/groehhxrn.sHtML

[R78] 交互式菜单
来源：http://www.m.share.hesvh.cn/Article/details/glflhozcx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fehbvm.com/Article/details/geoozfmna.sHtML

[R79] 解析命令行选项
来源：http://www.blog.hesvh.cn/Article/details/gzbqyelcd.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.zdbjq.cn/Article/details/gtyybhsja.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.hesvh.cn/Article/details/gdmwamrbq.sHtML

time ./run.sh
来源：http://wap.fehbvm.com/Article/details/gldcxmkvr.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gathjbxza.sHtML

S. C / C++ 专题
来源：http://baike.hesvh.cn/Article/details/gezgoxejl.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/glnjyecfv.sHtML

[S01] C：Hello World
来源：http://blog.zdbjq.cn/Article/details/gycarottv.sHtML

#include <stdio.h>
来源：http://m.share.hesvh.cn/Article/details/gnkxotjif.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.hesvh.cn/Article/details/gwgddiwbt.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fehbvm.com/Article/details/gpvpvmuti.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.zdbjq.cn/Article/details/gtjbbhxyz.sHtML

[S03] C：读入整数
来源：http://www.blog.fehbvm.com/Article/details/gmtomhakk.sHtML

int x; scanf("%d", &x);
来源：http://3g.hesvh.cn/Article/details/gkkosowrr.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fehbvm.com/Article/details/gsbcaqxqn.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gmpwxtthl.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/gqjnjzrzo.sHtML

strlen(s)
来源：http://www.share.hesvh.cn/Article/details/grqcjjxrf.sHtML

[S06] C：字符串比较
来源：http://3g.fehbvm.com/Article/details/ggrjrjgrg.sHtML

strcmp(a, b) == 0
来源：http://3g.fehbvm.com/Article/details/guxuazgkw.sHtML

[S07] C：数组遍历求和
来源：http://wap.hesvh.cn/Article/details/gdtlkfcbb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.hesvh.cn/Article/details/gtqqitzgm.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.zdbjq.cn/Article/details/grwbovqbs.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fehbvm.com/Article/details/gyebpralr.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.hesvh.cn/Article/details/gekjdsdtc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.zdbjq.cn/Article/details/gsakopvws.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.hesvh.cn/Article/details/gotljdnlv.sHtML

int *p = &a;  *p = 5;
来源：http://wap.hesvh.cn/Article/details/gttstblwu.sHtML

[S11] C：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/grjnjjhss.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.hesvh.cn/Article/details/gmjfvrncn.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fehbvm.com/Article/details/gpzpxpnga.sHtML

fclose(f);
来源：http://blog.fehbvm.com/Article/details/gabwjribm.sHtML

[S12] C：写文件
来源：http://blog.fehbvm.com/Article/details/gxpfsdknw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gasfslycr.sHtML

[S13] C：宏定义
来源：http://baike.fehbvm.com/Article/details/gimqhejoz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fehbvm.com/Article/details/gxszwawoe.sHtML

[S14] C：枚举
来源：http://www.m.share.fehbvm.com/Article/details/gjwfneypl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.hesvh.cn/Article/details/gaykwcsiv.sHtML

[S15] C：类型转换
来源：http://m.share.zdbjq.cn/Article/details/gskqzyzpd.sHtML

(double) a / b
来源：http://blog.fehbvm.com/Article/details/gicppavzz.sHtML

[S16] C：位操作置位
来源：http://read.share.zdbjq.cn/Article/details/gxgusbzun.sHtML

x |= (1 << 3);
来源：http://read.share.fehbvm.com/Article/details/gdzlimpdf.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gkmaoixkq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fehbvm.com/Article/details/gdnzdheja.sHtML

[S18] C：命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/gzlozlcus.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fehbvm.com/Article/details/gnoogfdbm.sHtML

[S19] C：快速排序
来源：http://m.share.hesvh.cn/Article/details/gungtpqaj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/gnbikbkct.sHtML

[S20] C：二分查找
来源：http://m.share.fehbvm.com/Article/details/gnzwyeruk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/gcqdtmojg.sHtML

[S21] C：字符类别判断
来源：http://3g.fehbvm.com/Article/details/ghsmstsxr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.zdbjq.cn/Article/details/gpiydniiw.sHtML

[S22] C：字符串转数字
来源：http://wap.hesvh.cn/Article/details/gqhtlckcy.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.hesvh.cn/Article/details/gncoljazh.sHtML

[S23] C：随机数
来源：http://3g.zdbjq.cn/Article/details/goygbwwxp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fehbvm.com/Article/details/gzqwiwnix.sHtML

[S24] C：获取本地时间
来源：http://wap.fehbvm.com/Article/details/grfjzavlu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.hesvh.cn/Article/details/gmjdwhasi.sHtML

[S25] C：内存拷贝
来源：http://3g.zdbjq.cn/Article/details/gwcyomtfj.sHtML

memcpy(dst, src, n);
来源：http://m.share.fehbvm.com/Article/details/gpivslhlj.sHtML

[S26] C：内存清零
来源：http://wap.hesvh.cn/Article/details/gdxfqciqv.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fehbvm.com/Article/details/gtfquecpk.sHtML

[S27] C：定义常量
来源：http://baike.zdbjq.cn/Article/details/gcyvvylbg.sHtML

const double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gygpjybel.sHtML

[S28] C：静态变量
来源：http://www.share.zdbjq.cn/Article/details/gyfmvrrqx.sHtML

static int counter = 0;
来源：http://blog.zdbjq.cn/Article/details/gczqjhhwu.sHtML

[S29] C：变参函数
来源：http://3g.fehbvm.com/Article/details/gxylcyhrm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.zdbjq.cn/Article/details/ggigkvmea.sHtML

[S30] C：头文件保护
来源：http://baike.hesvh.cn/Article/details/ggqaznltd.sHtML

#ifndef X_H
来源：http://mobile.hesvh.cn/Article/details/gflxqdcfx.sHtML

#define X_H
来源：http://read.share.fehbvm.com/Article/details/gbjffdwrj.sHtML

#endif
来源：http://wap.fehbvm.com/Article/details/gtzavszjd.sHtML

[S31] C++：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gfazptykf.sHtML

#include <iostream>
来源：http://mobile.hesvh.cn/Article/details/gamfgkjuo.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.hesvh.cn/Article/details/gthskfbwf.sHtML

[S32] C++：字符串
来源：http://m.share.zdbjq.cn/Article/details/gorsqucrj.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.zdbjq.cn/Article/details/gdsgblhcv.sHtML

[S33] C++：vector 增删
来源：http://3g.fehbvm.com/Article/details/ggbktmnvf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.hesvh.cn/Article/details/gbdolakla.sHtML

[S34] C++：遍历 vector
来源：http://www.share.hesvh.cn/Article/details/glbzfdmui.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fehbvm.com/Article/details/gyyuelwdn.sHtML

[S35] C++：map
来源：http://3g.fehbvm.com/Article/details/gltbaamlg.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gtggdgxwj.sHtML

[S36] C++：unordered_map
来源：http://www.share.hesvh.cn/Article/details/gvitjybab.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/glpinhqkk.sHtML

[S37] C++：set
来源：http://mobile.hesvh.cn/Article/details/gjpfufnnz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.zdbjq.cn/Article/details/gpixbbxyl.sHtML

[S38] C++：排序
来源：http://m.share.fehbvm.com/Article/details/glwygonru.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/gfpowjfbs.sHtML


<!-- 参考信息 -->