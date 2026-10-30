代发 wailian999

[Q67] 设置隔离级别
来源：http://mobile.zdbjq.cn/Article/details/gjxhrqjql.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fehbvm.com/Article/details/gzykmheie.sHtML

[Q68] 保存点
来源：http://blog.zdbjq.cn/Article/details/gwdayowii.sHtML

SAVEPOINT sp1;
来源：http://mobile.hesvh.cn/Article/details/gsaywcbuk.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fehbvm.com/Article/details/gbjztfhpr.sHtML

[Q69] 查看执行计划
来源：http://mobile.hesvh.cn/Article/details/gelodjdiv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.hesvh.cn/Article/details/gekkrgzeq.sHtML

[Q70] 更新统计信息
来源：http://www.blog.hesvh.cn/Article/details/gkrhdpxwp.sHtML

ANALYZE TABLE users;
来源：http://read.share.zdbjq.cn/Article/details/giqcexmno.sHtML

[Q71] 查看建表语句
来源：http://wap.zdbjq.cn/Article/details/gcrgilhhm.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.zdbjq.cn/Article/details/glizzqglg.sHtML

[Q72] 查看索引
来源：http://mobile.hesvh.cn/Article/details/gjqrcbyvu.sHtML

SHOW INDEX FROM users;
来源：http://mobile.hesvh.cn/Article/details/gjxsbmbco.sHtML

[Q73] 查看表状态
来源：http://www.share.hesvh.cn/Article/details/ggjiinxsk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fehbvm.com/Article/details/gzyuwnvea.sHtML

[Q74] 强制使用索引
来源：http://www.share.hesvh.cn/Article/details/giezsnyxi.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.hesvh.cn/Article/details/gfkvqicjx.sHtML

[Q75] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/gcytdezci.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gbmiqzjte.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.hesvh.cn/Article/details/gwyjfjvtz.sHtML

[Q76] 按天统计
来源：http://www.m.share.fehbvm.com/Article/details/gydkdegdg.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fehbvm.com/Article/details/gcybmvkww.sHtML

[Q77] 时间加减
来源：http://read.share.zdbjq.cn/Article/details/gkkxqcgrc.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.zdbjq.cn/Article/details/gginuwftg.sHtML

[Q78] 当前时间
来源：http://baike.zdbjq.cn/Article/details/ggjbmxptl.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.zdbjq.cn/Article/details/guavijyml.sHtML

[Q79] 字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/gucvpdoda.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fehbvm.com/Article/details/gjfmglnxt.sHtML

[Q80] 字符串截取
来源：http://www.m.share.zdbjq.cn/Article/details/gjadkeige.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gtydzgmyk.sHtML

[Q81] 字符串替换
来源：http://www.m.share.hesvh.cn/Article/details/gxhictswt.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gnqaxgity.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.zdbjq.cn/Article/details/gqlvxltla.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gyetzahhl.sHtML

[Q83] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/gugjsqqwx.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gucaliawv.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.hesvh.cn/Article/details/gfesdwwcu.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gjkmolblb.sHtML

[Q85] 数值取整
来源：http://www.share.zdbjq.cn/Article/details/gwziyvvsg.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.hesvh.cn/Article/details/gfhhmodfb.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.hesvh.cn/Article/details/gkaliubew.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.hesvh.cn/Article/details/gozpdmgrs.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.zdbjq.cn/Article/details/gxgzrsmgb.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.zdbjq.cn/Article/details/gqehvmwbq.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fehbvm.com/Article/details/gyuckjprz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.zdbjq.cn/Article/details/gtqfkloyp.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fehbvm.com/Article/details/goersseqo.sHtML

[Q89] 判断表是否存在
来源：http://www.share.hesvh.cn/Article/details/gplfhymtm.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.hesvh.cn/Article/details/grqigfftn.sHtML

[Q90] 生成序号列
来源：http://m.share.fehbvm.com/Article/details/ggnegwqyg.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fehbvm.com/Article/details/gpgmwpjyk.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gdrbdbyep.sHtML

R. Bash 专题
来源：http://mobile.hesvh.cn/Article/details/grqjnciah.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/grccibhzu.sHtML

[R01] shebang 与严格模式
来源：http://mobile.hesvh.cn/Article/details/gsrmfvaou.sHtML

#!/usr/bin/env bash
来源：http://wap.fehbvm.com/Article/details/gcytrvakq.sHtML

set -euo pipefail
来源：http://3g.zdbjq.cn/Article/details/gbqsyrash.sHtML

[R02] 变量赋值与使用
来源：http://mobile.zdbjq.cn/Article/details/ghwvbtrio.sHtML

name="Tom"; echo "$name"
来源：http://3g.fehbvm.com/Article/details/gfvlykjlf.sHtML

[R03] 只读变量
来源：http://read.share.hesvh.cn/Article/details/gqldknpea.sHtML

readonly PI=3.14
来源：http://mobile.hesvh.cn/Article/details/ghwxppsqh.sHtML

[R04] 位置参数
来源：http://www.blog.zdbjq.cn/Article/details/gjvumgmdn.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fehbvm.com/Article/details/gzqvhzghp.sHtML

[R05] 参数默认值
来源：http://baike.hesvh.cn/Article/details/ghuxaathw.sHtML

name="${1:-default}"
来源：http://wap.zdbjq.cn/Article/details/geieazfzl.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gsiwrsygb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/gdndxldmh.sHtML

[R07] if 判断文件
来源：http://read.share.hesvh.cn/Article/details/gfnxpzwij.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.zdbjq.cn/Article/details/guqrkldpn.sHtML

[R08] 数值比较
来源：http://www.m.share.fehbvm.com/Article/details/gbkqbgxgu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.zdbjq.cn/Article/details/gpzppirlq.sHtML

[R09] 字符串比较
来源：http://baike.fehbvm.com/Article/details/gobfnqrll.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.zdbjq.cn/Article/details/gpzqqwlfc.sHtML

[R10] 正则匹配
来源：http://mobile.zdbjq.cn/Article/details/gajpxwfww.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fehbvm.com/Article/details/gpqjjgqot.sHtML

[R11] case 多分支
来源：http://read.share.hesvh.cn/Article/details/gbwrrizdz.sHtML

case "$1" in
来源：http://mobile.hesvh.cn/Article/details/gwchzaimz.sHtML

start) echo "启动" ;;
来源：http://www.blog.fehbvm.com/Article/details/gevgqtvth.sHtML

stop)  echo "停止" ;;
来源：http://www.share.zdbjq.cn/Article/details/gzswiovij.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gdwpefwhf.sHtML

esac
来源：http://www.m.share.hesvh.cn/Article/details/gewfazqlx.sHtML

[R12] for 遍历文件
来源：http://www.share.zdbjq.cn/Article/details/gwrwrfkmz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.hesvh.cn/Article/details/gabncppym.sHtML

[R13] for 计数循环
来源：http://blog.fehbvm.com/Article/details/gmvvpbnom.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gguuecvyb.sHtML

[R14] C 风格 for
来源：http://baike.fehbvm.com/Article/details/gmkbwlflu.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/gagtmxcdz.sHtML

[R15] while 逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gcvsctreq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fehbvm.com/Article/details/gxzhtrike.sHtML

[R16] until 等待条件
来源：http://blog.zdbjq.cn/Article/details/gihtxlbbn.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gbjbsfdoh.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.hesvh.cn/Article/details/gbysdglpw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.zdbjq.cn/Article/details/gkxfjcjea.sHtML

[R18] 遍历数组
来源：http://www.share.hesvh.cn/Article/details/gvmfbapok.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.hesvh.cn/Article/details/gmhyuizzs.sHtML

[R19] 数组长度
来源：http://read.share.fehbvm.com/Article/details/gnfbojtcn.sHtML

echo "${#arr[@]}"
来源：http://3g.zdbjq.cn/Article/details/goqtpuvoa.sHtML

[R20] 关联数组（字典）
来源：http://wap.fehbvm.com/Article/details/gpgomigjh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.hesvh.cn/Article/details/grdaiqbrp.sHtML

[R21] 字符串长度
来源：http://3g.zdbjq.cn/Article/details/gbfbpcxil.sHtML

echo "${#s}"
来源：http://read.share.hesvh.cn/Article/details/gpavqpcfv.sHtML

[R22] 截取子串
来源：http://www.m.share.fehbvm.com/Article/details/gsetckdhy.sHtML

echo "${s:0:5}"
来源：http://www.share.fehbvm.com/Article/details/glafquoas.sHtML

[R23] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gixygfnkw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fehbvm.com/Article/details/gkviyntfp.sHtML

[R24] 大小写转换
来源：http://3g.hesvh.cn/Article/details/gjxtfonmn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fehbvm.com/Article/details/gqdcycghw.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fehbvm.com/Article/details/glgwqidqm.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fehbvm.com/Article/details/gvpfqzumv.sHtML

[R26] 命令替换
来源：http://m.share.hesvh.cn/Article/details/gegnczuaf.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.zdbjq.cn/Article/details/goknftogr.sHtML

[R27] 算术展开
来源：http://wap.zdbjq.cn/Article/details/gpvpyvhgl.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fehbvm.com/Article/details/gcamrzovh.sHtML

[R28] 浮点运算
来源：http://blog.fehbvm.com/Article/details/gzbaffell.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.zdbjq.cn/Article/details/gnvlsrwwc.sHtML

[R29] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/gqbkytunw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.hesvh.cn/Article/details/gknldqxng.sHtML

[R30] 函数返回状态码
来源：http://www.blog.hesvh.cn/Article/details/gjufrvrgx.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.hesvh.cn/Article/details/gjmsatqyu.sHtML

[R31] 局部变量
来源：http://3g.zdbjq.cn/Article/details/giejniezg.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fehbvm.com/Article/details/grdmmgzpq.sHtML

[R32] 参数个数校验
来源：http://m.share.fehbvm.com/Article/details/gicqfhvbf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/goovesjtx.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fehbvm.com/Article/details/gyryjcyba.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.hesvh.cn/Article/details/gcnoclwtp.sHtML

[R34] 退出时清理
来源：http://m.share.hesvh.cn/Article/details/gigpgvzyn.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/gpezenvgd.sHtML

[R35] 后台执行并等待
来源：http://m.share.hesvh.cn/Article/details/goczazynm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fehbvm.com/Article/details/goaaxeqte.sHtML

[R36] 并发执行多个任务
来源：http://baike.zdbjq.cn/Article/details/gpqbpekrm.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fehbvm.com/Article/details/gmcyhblbi.sHtML

[R37] 把输出赋给变量
来源：http://3g.hesvh.cn/Article/details/gsmgazuxp.sHtML

files=$(ls -1)
来源：http://m.share.zdbjq.cn/Article/details/gjfodhjiw.sHtML

[R38] 管道串联
来源：http://3g.hesvh.cn/Article/details/gceduhkto.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fehbvm.com/Article/details/gxkldixeh.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.hesvh.cn/Article/details/gqoigcqel.sHtML

cmd > out.log 2>&1
来源：http://3g.fehbvm.com/Article/details/gzqhgnkqs.sHtML

[R40] 追加写日志
来源：http://blog.zdbjq.cn/Article/details/gdjpgapzf.sHtML

echo "log" >> out.log
来源：http://blog.hesvh.cn/Article/details/gnijzauzb.sHtML

[R41] 丢弃输出
来源：http://wap.fehbvm.com/Article/details/gjnwlvofi.sHtML

cmd >/dev/null 2>&1
来源：http://baike.zdbjq.cn/Article/details/goxdcxocr.sHtML

[R42] 输入重定向
来源：http://blog.hesvh.cn/Article/details/gniodxakp.sHtML

wc -l < a.txt
来源：http://m.share.hesvh.cn/Article/details/ggsmsnqmv.sHtML

[R43] 按名字查找文件
来源：http://read.share.hesvh.cn/Article/details/gdcwtzccq.sHtML

find . -name "*.log" -type f
来源：http://www.blog.zdbjq.cn/Article/details/guwjjalti.sHtML

[R44] 按修改时间查找
来源：http://3g.hesvh.cn/Article/details/gqncmgqek.sHtML

find . -mtime -7 -type f
来源：http://baike.fehbvm.com/Article/details/grhgubadi.sHtML

[R45] 批量删除
来源：http://www.share.hesvh.cn/Article/details/gdjetsvzh.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fehbvm.com/Article/details/gekeugphh.sHtML

[R46] 递归替换文件内容
来源：http://baike.zdbjq.cn/Article/details/gppjapeif.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fehbvm.com/Article/details/gheevupvs.sHtML

[R47] sed 单行替换
来源：http://read.share.fehbvm.com/Article/details/gywnfihwa.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fehbvm.com/Article/details/gjkjomvwm.sHtML

[R48] awk 取指定列
来源：http://mobile.fehbvm.com/Article/details/gowzaxtel.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gtrmtqfxw.sHtML

[R49] awk 带条件
来源：http://read.share.hesvh.cn/Article/details/gtzgeaptz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fehbvm.com/Article/details/gfgvvrnuh.sHtML

[R50] awk 求和
来源：http://3g.zdbjq.cn/Article/details/gssffrhvy.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.hesvh.cn/Article/details/gqwybntzo.sHtML

[R51] 排序去重取前几
来源：http://mobile.fehbvm.com/Article/details/gtuwrxczx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.hesvh.cn/Article/details/gphzbahcg.sHtML

[R52] 统计行数
来源：http://blog.zdbjq.cn/Article/details/gnashbfcv.sHtML

wc -l a.txt
来源：http://mobile.hesvh.cn/Article/details/gclibeflm.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fehbvm.com/Article/details/gshhssyve.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.zdbjq.cn/Article/details/gbupqdrvn.sHtML

[R54] 比较两个文件
来源：http://blog.hesvh.cn/Article/details/goglwjgtz.sHtML

diff a.txt b.txt
来源：http://blog.hesvh.cn/Article/details/glcohlzyb.sHtML

[R55] 压缩与解压
来源：http://baike.zdbjq.cn/Article/details/gxlyoiuzo.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.hesvh.cn/Article/details/ghbiywnpm.sHtML

[R56] 远程拷贝
来源：http://wap.hesvh.cn/Article/details/gistpaiqc.sHtML

scp file user@host:/path/
来源：http://www.share.zdbjq.cn/Article/details/gelvxrzsk.sHtML

[R57] 远程执行命令
来源：http://mobile.zdbjq.cn/Article/details/gfxjpnige.sHtML

ssh user@host 'uptime'
来源：http://www.share.zdbjq.cn/Article/details/gsdgjhvgz.sHtML

[R58] 下载文件
来源：http://www.m.share.zdbjq.cn/Article/details/gipbphtsz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.hesvh.cn/Article/details/gekkiorwd.sHtML

[R59] 发 POST JSON
来源：http://m.share.fehbvm.com/Article/details/gaxqkgbyu.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.hesvh.cn/Article/details/gsluqcjut.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.hesvh.cn/Article/details/geknkjreq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.zdbjq.cn/Article/details/giklyuxms.sHtML

[R61] 磁盘占用
来源：http://blog.hesvh.cn/Article/details/gmmsnjpbw.sHtML

df -h;  du -sh *
来源：http://baike.hesvh.cn/Article/details/gstmakkbz.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.zdbjq.cn/Article/details/ghqsabxce.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fehbvm.com/Article/details/gwntyfvjp.sHtML

[R63] 内存与进程
来源：http://www.blog.fehbvm.com/Article/details/grguknypg.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.hesvh.cn/Article/details/givulrljo.sHtML

[R64] 结束进程
来源：http://www.blog.fehbvm.com/Article/details/gfkouhpby.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.hesvh.cn/Article/details/gsscgrkor.sHtML

[R65] 查看端口占用
来源：http://www.share.zdbjq.cn/Article/details/ggurcnbxt.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.zdbjq.cn/Article/details/gthitcvfz.sHtML

[R66] 定时任务
来源：http://wap.hesvh.cn/Article/details/gwhznygzz.sHtML

crontab -e;  crontab -l
来源：http://baike.zdbjq.cn/Article/details/gzchgsvcu.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fehbvm.com/Article/details/ghkmqgpcy.sHtML

openssl rand -hex 16
来源：http://www.blog.zdbjq.cn/Article/details/gkqgcnesh.sHtML

[R68] 计算文件校验值
来源：http://read.share.hesvh.cn/Article/details/gomwrnqca.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fehbvm.com/Article/details/gzamzzjgf.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fehbvm.com/Article/details/grclqipln.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.zdbjq.cn/Article/details/gsnxmtkjy.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fehbvm.com/Article/details/gkytfhcua.sHtML

date +%s;  date -d @1700000000
来源：http://blog.hesvh.cn/Article/details/gsewjtiva.sHtML

[R71] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/gfaauriei.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.hesvh.cn/Article/details/gtjegadwz.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fehbvm.com/Article/details/gsptrwkej.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/gkkayiwxe.sHtML

[R73] 分割大日志
来源：http://read.share.hesvh.cn/Article/details/glrdbgkxs.sHtML

split -l 1000 big.log part_
来源：http://3g.fehbvm.com/Article/details/gcaycoebk.sHtML

[R74] 批量重命名
来源：http://www.blog.zdbjq.cn/Article/details/gnjuqefuf.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.zdbjq.cn/Article/details/gwnxaswez.sHtML

[R75] 导出环境变量
来源：http://blog.fehbvm.com/Article/details/gfheodzrq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.hesvh.cn/Article/details/gaykfyonq.sHtML

[R76] 使用临时文件
来源：http://read.share.hesvh.cn/Article/details/gldpltvna.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gotbuviig.sHtML

[R77] 读取用户输入
来源：http://www.blog.zdbjq.cn/Article/details/gozzoiydq.sHtML

read -rp "请输入: " ans
来源：http://wap.hesvh.cn/Article/details/gaeitnrxl.sHtML

[R78] 交互式菜单
来源：http://wap.zdbjq.cn/Article/details/gwgnudzsm.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.zdbjq.cn/Article/details/gyeinnqhk.sHtML

[R79] 解析命令行选项
来源：http://wap.hesvh.cn/Article/details/giwfxqgnv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.hesvh.cn/Article/details/gmczimgxi.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.zdbjq.cn/Article/details/gsxcigxkq.sHtML

time ./run.sh
来源：http://wap.zdbjq.cn/Article/details/gjesmzjji.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gcgxulaci.sHtML

S. C / C++ 专题
来源：http://www.blog.hesvh.cn/Article/details/grdzmcnmg.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ghndpnhtr.sHtML

[S01] C：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gwvfbmddc.sHtML

#include <stdio.h>
来源：http://3g.zdbjq.cn/Article/details/gvvjblviv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.hesvh.cn/Article/details/godfpsrrn.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.zdbjq.cn/Article/details/gjrvricly.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.zdbjq.cn/Article/details/gftnucyrp.sHtML

[S03] C：读入整数
来源：http://www.blog.hesvh.cn/Article/details/gwwkznszk.sHtML

int x; scanf("%d", &x);
来源：http://3g.zdbjq.cn/Article/details/gvtvkxxvk.sHtML

[S04] C：字符串复制
来源：http://www.m.share.hesvh.cn/Article/details/gxgjcnrrs.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.zdbjq.cn/Article/details/gckldxeol.sHtML

[S05] C：字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/gbqbgvfak.sHtML

strlen(s)
来源：http://www.share.fehbvm.com/Article/details/gkfccfzzi.sHtML

[S06] C：字符串比较
来源：http://blog.zdbjq.cn/Article/details/gpugmrudp.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fehbvm.com/Article/details/glugrqsqx.sHtML

[S07] C：数组遍历求和
来源：http://m.share.hesvh.cn/Article/details/gdgstdkba.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.hesvh.cn/Article/details/gshnlkczq.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.zdbjq.cn/Article/details/gcidrojbh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fehbvm.com/Article/details/gsjcyntpd.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.zdbjq.cn/Article/details/gcjyrsaiq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fehbvm.com/Article/details/gfjnfxajh.sHtML

[S10] C：指针与解引用
来源：http://wap.zdbjq.cn/Article/details/gnlgzvdqj.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.hesvh.cn/Article/details/gyhkdjmzg.sHtML

[S11] C：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gxsnxgcnt.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.zdbjq.cn/Article/details/gmsibwcsk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.zdbjq.cn/Article/details/gilamtojb.sHtML

fclose(f);
来源：http://3g.fehbvm.com/Article/details/gczwgmyhs.sHtML

[S12] C：写文件
来源：http://m.share.zdbjq.cn/Article/details/geylaremn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.hesvh.cn/Article/details/gzgvkdjhr.sHtML

[S13] C：宏定义
来源：http://www.m.share.hesvh.cn/Article/details/gqamagtdk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.zdbjq.cn/Article/details/gmjxehizz.sHtML

[S14] C：枚举
来源：http://mobile.zdbjq.cn/Article/details/grpuylsku.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.zdbjq.cn/Article/details/ggjdutkqg.sHtML

[S15] C：类型转换
来源：http://www.m.share.hesvh.cn/Article/details/gpdrqfkvx.sHtML

(double) a / b
来源：http://www.share.hesvh.cn/Article/details/gauovpxto.sHtML

[S16] C：位操作置位
来源：http://blog.fehbvm.com/Article/details/gwmygngxp.sHtML

x |= (1 << 3);
来源：http://www.m.share.hesvh.cn/Article/details/gvddsgjag.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gzbcvaqad.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fehbvm.com/Article/details/gbvyljzcb.sHtML

[S18] C：命令行参数
来源：http://3g.fehbvm.com/Article/details/gsrkplhns.sHtML

int main(int argc, char **argv)
来源：http://baike.fehbvm.com/Article/details/gqrezmqvx.sHtML

[S19] C：快速排序
来源：http://3g.fehbvm.com/Article/details/gbxfziowx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/gkwayywgv.sHtML

[S20] C：二分查找
来源：http://blog.zdbjq.cn/Article/details/gupdxvoms.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/golajfkwc.sHtML

[S21] C：字符类别判断
来源：http://blog.fehbvm.com/Article/details/gvttvspky.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.hesvh.cn/Article/details/gtqrgkvcm.sHtML

[S22] C：字符串转数字
来源：http://3g.fehbvm.com/Article/details/gyhunydof.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fehbvm.com/Article/details/gkvgdiqay.sHtML

[S23] C：随机数
来源：http://www.blog.hesvh.cn/Article/details/gdrigdjps.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.hesvh.cn/Article/details/gusjxwfmf.sHtML

[S24] C：获取本地时间
来源：http://www.share.fehbvm.com/Article/details/gnvwaisot.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.zdbjq.cn/Article/details/gwshcvmuw.sHtML

[S25] C：内存拷贝
来源：http://baike.fehbvm.com/Article/details/gvmwhtdus.sHtML

memcpy(dst, src, n);
来源：http://www.blog.zdbjq.cn/Article/details/gsxblkczt.sHtML

[S26] C：内存清零
来源：http://www.share.hesvh.cn/Article/details/goqioirya.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.zdbjq.cn/Article/details/gmnqolgit.sHtML

[S27] C：定义常量
来源：http://3g.fehbvm.com/Article/details/gqxndzmtm.sHtML

const double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gjxrrprgu.sHtML

[S28] C：静态变量
来源：http://www.share.hesvh.cn/Article/details/grvnxpckh.sHtML

static int counter = 0;
来源：http://www.m.share.zdbjq.cn/Article/details/gslnetbdb.sHtML

[S29] C：变参函数
来源：http://www.blog.zdbjq.cn/Article/details/gfpjreawr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.hesvh.cn/Article/details/gxcvckncn.sHtML

[S30] C：头文件保护
来源：http://www.blog.zdbjq.cn/Article/details/gnnxvmfnr.sHtML

#ifndef X_H
来源：http://3g.zdbjq.cn/Article/details/ghlzhcfqg.sHtML

#define X_H
来源：http://read.share.zdbjq.cn/Article/details/gezykdkan.sHtML

#endif
来源：http://baike.zdbjq.cn/Article/details/gzyrsmeyo.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gklvjufiw.sHtML

#include <iostream>
来源：http://baike.zdbjq.cn/Article/details/guluqvxud.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fehbvm.com/Article/details/gdzjmbmfa.sHtML

[S32] C++：字符串
来源：http://m.share.zdbjq.cn/Article/details/gvtglwjzs.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.hesvh.cn/Article/details/gjhmyvawz.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.zdbjq.cn/Article/details/gykzeldad.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.hesvh.cn/Article/details/gnekcizre.sHtML

[S34] C++：遍历 vector
来源：http://3g.fehbvm.com/Article/details/gedhqddey.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.zdbjq.cn/Article/details/gewolpihn.sHtML

[S35] C++：map
来源：http://m.share.zdbjq.cn/Article/details/gcgnerylh.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gibtjplpg.sHtML

[S36] C++：unordered_map
来源：http://www.blog.zdbjq.cn/Article/details/ghrgnuiqw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fehbvm.com/Article/details/giabqrkii.sHtML


<!-- 参考信息 -->