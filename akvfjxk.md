代发 wailian999

SHOW INDEX FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvomdcdct.sHtML

[Q73] 查看表状态
来源：http://baike.fanxiaobao.xyz/Article/details/gljqvaarj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/goiznvvlo.sHtML

[Q74] 强制使用索引
来源：http://blog.fanxiaobao.xyz/Article/details/gjbophxpj.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fanxiaobao.xyz/Article/details/gyvizpwai.sHtML

[Q75] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gqohzqgat.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gzaptktcy.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggltkffdd.sHtML

[Q76] 按天统计
来源：http://3g.fanxiaobao.xyz/Article/details/gmxdwddlx.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbnqeqxzd.sHtML

[Q77] 时间加减
来源：http://mobile.fanxiaobao.xyz/Article/details/gvdcrsjkq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fanxiaobao.xyz/Article/details/gtfxhgvqf.sHtML

[Q78] 当前时间
来源：http://wap.fanxiaobao.xyz/Article/details/gawgnkfbq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fanxiaobao.xyz/Article/details/gyyykdzft.sHtML

[Q79] 字符串拼接
来源：http://read.share.fanxiaobao.xyz/Article/details/gsapjkhlh.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmlnavzwd.sHtML

[Q80] 字符串截取
来源：http://baike.fanxiaobao.xyz/Article/details/gpoylzysi.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gltquyfkz.sHtML

[Q81] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/giojwktil.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnqsrqydi.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fanxiaobao.xyz/Article/details/gsoxligwa.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gzptdzvbl.sHtML

[Q83] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gzvsohiig.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkehrflso.sHtML

[Q84] 去除首尾空格
来源：http://blog.fanxiaobao.xyz/Article/details/gleiykoak.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtepvtpjd.sHtML

[Q85] 数值取整
来源：http://mobile.fanxiaobao.xyz/Article/details/gyrzartgj.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fanxiaobao.xyz/Article/details/genzeeqik.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fanxiaobao.xyz/Article/details/gnakttjql.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gthmqprru.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fanxiaobao.xyz/Article/details/grpfwzqli.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzhkqwcae.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fanxiaobao.xyz/Article/details/gsvcnjvuj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fanxiaobao.xyz/Article/details/gevexbbqf.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gqrjfathg.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gkudovikh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvtjgbnlh.sHtML

[Q90] 生成序号列
来源：http://www.blog.fanxiaobao.xyz/Article/details/goaaxwrly.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqotejfux.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gdbiczvon.sHtML

R. Bash 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gfftrwdjy.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gapodqdbk.sHtML

[R01] shebang 与严格模式
来源：http://baike.fanxiaobao.xyz/Article/details/gavmfoztl.sHtML

#!/usr/bin/env bash
来源：http://read.share.fanxiaobao.xyz/Article/details/geoywgyio.sHtML

set -euo pipefail
来源：http://www.share.fanxiaobao.xyz/Article/details/ghxjcuome.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggyqxmftq.sHtML

name="Tom"; echo "$name"
来源：http://3g.fanxiaobao.xyz/Article/details/gitrrwexo.sHtML

[R03] 只读变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpxzktjxc.sHtML

readonly PI=3.14
来源：http://blog.fanxiaobao.xyz/Article/details/gjkbnsjfg.sHtML

[R04] 位置参数
来源：http://wap.fanxiaobao.xyz/Article/details/gwmyvmhtb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwqmvewfx.sHtML

[R05] 参数默认值
来源：http://blog.fanxiaobao.xyz/Article/details/gvkwfthsd.sHtML

name="${1:-default}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsxodauwr.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzduzsegb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gpvzamymo.sHtML

[R07] if 判断文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggaxjmnnj.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gpbipmyvw.sHtML

[R08] 数值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gypjjuvjy.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gunkeothh.sHtML

[R09] 字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gscdtaiuj.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gzdlklcfg.sHtML

[R10] 正则匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gjohkdscu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gmtdhfyth.sHtML

[R11] case 多分支
来源：http://3g.fanxiaobao.xyz/Article/details/gjrgoqups.sHtML

case "$1" in
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvxdfxcn.sHtML

start) echo "启动" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gctghdvoq.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkkmujjbz.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghoengfxg.sHtML

esac
来源：http://www.share.fanxiaobao.xyz/Article/details/gkposagnd.sHtML

[R12] for 遍历文件
来源：http://baike.fanxiaobao.xyz/Article/details/gegpczpff.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fanxiaobao.xyz/Article/details/ggmsvtfcy.sHtML

[R13] for 计数循环
来源：http://blog.fanxiaobao.xyz/Article/details/gzooqqpom.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbfzwuins.sHtML

[R14] C 风格 for
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkvysybbt.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gwhwqhydt.sHtML

[R15] while 逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/grapitkpg.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gugrpoqjs.sHtML

[R16] until 等待条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gkyxspmou.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gsiotimsf.sHtML

[R17] 数组定义与取值
来源：http://baike.fanxiaobao.xyz/Article/details/gozvqczcn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzpczuvoz.sHtML

[R18] 遍历数组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsfhahqcj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gjxbusitm.sHtML

[R19] 数组长度
来源：http://blog.fanxiaobao.xyz/Article/details/gyjlrfagx.sHtML

echo "${#arr[@]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/guliqcgub.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gckawithn.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gbcljqysi.sHtML

[R21] 字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gmrynmbdn.sHtML

echo "${#s}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gnsogjmbx.sHtML

[R22] 截取子串
来源：http://mobile.fanxiaobao.xyz/Article/details/gdsutsyly.sHtML

echo "${s:0:5}"
来源：http://www.share.fanxiaobao.xyz/Article/details/govjcufnu.sHtML

[R23] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gmumldqfp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gemnthucw.sHtML

[R24] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gkoehuaqk.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gezkvjkfh.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwepeumff.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fanxiaobao.xyz/Article/details/ggrapphup.sHtML

[R26] 命令替换
来源：http://m.share.fanxiaobao.xyz/Article/details/grvobvion.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fanxiaobao.xyz/Article/details/grxdcrfit.sHtML

[R27] 算术展开
来源：http://3g.fanxiaobao.xyz/Article/details/gjaxlwvjs.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fanxiaobao.xyz/Article/details/gngyctxfl.sHtML

[R28] 浮点运算
来源：http://www.blog.fanxiaobao.xyz/Article/details/glbymmvnc.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhdzybka.sHtML

[R29] 定义函数
来源：http://baike.fanxiaobao.xyz/Article/details/gmzksprje.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fanxiaobao.xyz/Article/details/gopdhgjnp.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhyzzsiz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fanxiaobao.xyz/Article/details/gpodulmvu.sHtML

[R31] 局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcrshmlqh.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gpkhkrady.sHtML

[R32] 参数个数校验
来源：http://mobile.fanxiaobao.xyz/Article/details/gejcghffb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxgxlchm.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfdsvhkxx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fanxiaobao.xyz/Article/details/gsthufqly.sHtML

[R34] 退出时清理
来源：http://www.share.fanxiaobao.xyz/Article/details/gypoccguj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gwyyxmhae.sHtML

[R35] 后台执行并等待
来源：http://read.share.fanxiaobao.xyz/Article/details/gbqfbqviv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fanxiaobao.xyz/Article/details/gwspmjgig.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goyzyzmma.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/gplrcotwu.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbtjcczta.sHtML

files=$(ls -1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gburveqdj.sHtML

[R38] 管道串联
来源：http://wap.fanxiaobao.xyz/Article/details/gfenungro.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fanxiaobao.xyz/Article/details/gfplbyfam.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fanxiaobao.xyz/Article/details/gxudwihxe.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gszoehofa.sHtML

[R40] 追加写日志
来源：http://wap.fanxiaobao.xyz/Article/details/geqnbxfzk.sHtML

echo "log" >> out.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gekzairhs.sHtML

[R41] 丢弃输出
来源：http://baike.fanxiaobao.xyz/Article/details/ggtdvdtag.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gfywjcyhz.sHtML

[R42] 输入重定向
来源：http://baike.fanxiaobao.xyz/Article/details/gabkvqbuu.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnwgjtkfq.sHtML

[R43] 按名字查找文件
来源：http://blog.fanxiaobao.xyz/Article/details/gudveynvy.sHtML

find . -name "*.log" -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gxbhtihae.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjullzbc.sHtML

find . -mtime -7 -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gnnjeltlp.sHtML

[R45] 批量删除
来源：http://www.share.fanxiaobao.xyz/Article/details/gcmqrixti.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fanxiaobao.xyz/Article/details/glulwtjtz.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fanxiaobao.xyz/Article/details/gdwnasglt.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fanxiaobao.xyz/Article/details/gktdaxtof.sHtML

[R47] sed 单行替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gpddrgswx.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gknhffayh.sHtML

[R48] awk 取指定列
来源：http://mobile.fanxiaobao.xyz/Article/details/gmydxrjud.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gdufoxenq.sHtML

[R49] awk 带条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gamcihztc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fanxiaobao.xyz/Article/details/gexjiuiwe.sHtML

[R50] awk 求和
来源：http://wap.fanxiaobao.xyz/Article/details/gdkaxvgvr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gbciuhpuv.sHtML

[R51] 排序去重取前几
来源：http://blog.fanxiaobao.xyz/Article/details/gvksogmup.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fanxiaobao.xyz/Article/details/gvstbecec.sHtML

[R52] 统计行数
来源：http://www.share.fanxiaobao.xyz/Article/details/gxszhcjlz.sHtML

wc -l a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gbyrcuefr.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fanxiaobao.xyz/Article/details/gwwmhhlre.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gttivruvt.sHtML

[R54] 比较两个文件
来源：http://baike.fanxiaobao.xyz/Article/details/gxmkhxyxc.sHtML

diff a.txt b.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gyyyoynqb.sHtML

[R55] 压缩与解压
来源：http://mobile.fanxiaobao.xyz/Article/details/geekjuqrp.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fanxiaobao.xyz/Article/details/gttcwpznm.sHtML

[R56] 远程拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gtcwrbpoi.sHtML

scp file user@host:/path/
来源：http://www.share.fanxiaobao.xyz/Article/details/gljnqjsyp.sHtML

[R57] 远程执行命令
来源：http://mobile.fanxiaobao.xyz/Article/details/gqwsuneqm.sHtML

ssh user@host 'uptime'
来源：http://3g.fanxiaobao.xyz/Article/details/gwpbxcsvp.sHtML

[R58] 下载文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsztofise.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/guqgerpgc.sHtML

[R59] 发 POST JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gkvrgbcxx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fanxiaobao.xyz/Article/details/geuafhsgl.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhmdvduo.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gcsdkmixy.sHtML

[R61] 磁盘占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvzmaxwi.sHtML

df -h;  du -sh *
来源：http://3g.fanxiaobao.xyz/Article/details/gzwcfygwy.sHtML

[R62] 找最占空间的文件
来源：http://baike.fanxiaobao.xyz/Article/details/gacbiyswc.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/gbkqdyuza.sHtML

[R63] 内存与进程
来源：http://mobile.fanxiaobao.xyz/Article/details/ggaafgoag.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fanxiaobao.xyz/Article/details/gfcgmxqag.sHtML

[R64] 结束进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsokohqee.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fanxiaobao.xyz/Article/details/gcwwlxxzu.sHtML

[R65] 查看端口占用
来源：http://mobile.fanxiaobao.xyz/Article/details/ggnojkvwg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvrglplk.sHtML

[R66] 定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gwbzlzwxp.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdrjgerlp.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gahmgdhsl.sHtML

openssl rand -hex 16
来源：http://baike.fanxiaobao.xyz/Article/details/gymuyjmqu.sHtML

[R68] 计算文件校验值
来源：http://m.share.fanxiaobao.xyz/Article/details/gvqafmtne.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gyfiddjan.sHtML

[R69] 生成随机密码
来源：http://mobile.fanxiaobao.xyz/Article/details/gixvxaucr.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fanxiaobao.xyz/Article/details/gaprjqyza.sHtML

[R70] 时间戳与互转
来源：http://read.share.fanxiaobao.xyz/Article/details/gogvinlpb.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fanxiaobao.xyz/Article/details/gtptkxxvf.sHtML

[R71] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gqbmpzjqv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gviqzhpov.sHtML

[R72] 等待端口就绪
来源：http://3g.fanxiaobao.xyz/Article/details/gzpcbgeyn.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzhriqfly.sHtML

[R73] 分割大日志
来源：http://3g.fanxiaobao.xyz/Article/details/geyhpbxxz.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwcyrogxu.sHtML

[R74] 批量重命名
来源：http://wap.fanxiaobao.xyz/Article/details/gqrtkeqjl.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gorogwdag.sHtML

[R75] 导出环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/ggjbvcddf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fanxiaobao.xyz/Article/details/gbpuxutoo.sHtML

[R76] 使用临时文件
来源：http://m.share.fanxiaobao.xyz/Article/details/ghrwjrnte.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/glzdwbboe.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvtoattao.sHtML

read -rp "请输入: " ans
来源：http://3g.fanxiaobao.xyz/Article/details/gkltvfsqm.sHtML

[R78] 交互式菜单
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkspcujeq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fanxiaobao.xyz/Article/details/gaqmzlhsa.sHtML

[R79] 解析命令行选项
来源：http://www.share.fanxiaobao.xyz/Article/details/gubuphwtn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fanxiaobao.xyz/Article/details/goynscchz.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glwwmuboi.sHtML

time ./run.sh
来源：http://m.share.fanxiaobao.xyz/Article/details/gdqpubagl.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gakmjsgua.sHtML

S. C / C++ 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gsxooxkaz.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/geszgudon.sHtML

[S01] C：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gqrszxfus.sHtML

#include <stdio.h>
来源：http://blog.fanxiaobao.xyz/Article/details/glonboozs.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fanxiaobao.xyz/Article/details/gdkcjveug.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmddacmjx.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fanxiaobao.xyz/Article/details/ggqstgsnc.sHtML

[S03] C：读入整数
来源：http://baike.fanxiaobao.xyz/Article/details/gazgjstyh.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzmfibptc.sHtML

[S04] C：字符串复制
来源：http://mobile.fanxiaobao.xyz/Article/details/gunqzyhix.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/giboxxcmi.sHtML

[S05] C：字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/ghhrmfvgk.sHtML

strlen(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gekurxmmk.sHtML

[S06] C：字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gyvuhrmzh.sHtML

strcmp(a, b) == 0
来源：http://www.share.fanxiaobao.xyz/Article/details/gdyzesbta.sHtML

[S07] C：数组遍历求和
来源：http://blog.fanxiaobao.xyz/Article/details/grfvvagdx.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fanxiaobao.xyz/Article/details/gooojvqxm.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fanxiaobao.xyz/Article/details/gxpcnlbeq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fanxiaobao.xyz/Article/details/gxbcqgloz.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fanxiaobao.xyz/Article/details/gsgowvzfl.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdeihdmel.sHtML

[S10] C：指针与解引用
来源：http://m.share.fanxiaobao.xyz/Article/details/gdzvwpyul.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fanxiaobao.xyz/Article/details/gxmkcuqcf.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gqyajgxut.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fanxiaobao.xyz/Article/details/gyvyvkwrg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gzmohsvvo.sHtML

fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfujvxdcv.sHtML

[S12] C：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/glmdecgtw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/ghsxnezhl.sHtML

[S13] C：宏定义
来源：http://wap.fanxiaobao.xyz/Article/details/gbuekgxqh.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gujfighos.sHtML

[S14] C：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gutdwnbqb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fanxiaobao.xyz/Article/details/gyentqlps.sHtML

[S15] C：类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnyzvhwev.sHtML

(double) a / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gadoaojec.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsuyrhkok.sHtML

x |= (1 << 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvuujpovo.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gnbrpmslh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghgwcewzu.sHtML

[S18] C：命令行参数
来源：http://mobile.fanxiaobao.xyz/Article/details/ghocmzund.sHtML

int main(int argc, char **argv)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxdlbkeqr.sHtML

[S19] C：快速排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gxeytxgze.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gukmndvbs.sHtML

[S20] C：二分查找
来源：http://blog.fanxiaobao.xyz/Article/details/gyljkhgfm.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gjqxpssmx.sHtML

[S21] C：字符类别判断
来源：http://wap.fanxiaobao.xyz/Article/details/ghxvnzoel.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fanxiaobao.xyz/Article/details/gjwylcnbo.sHtML

[S22] C：字符串转数字
来源：http://baike.fanxiaobao.xyz/Article/details/gvfekagst.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fanxiaobao.xyz/Article/details/gljsgmooq.sHtML

[S23] C：随机数
来源：http://m.share.fanxiaobao.xyz/Article/details/gfuiuwwps.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghazoazeb.sHtML

[S24] C：获取本地时间
来源：http://baike.fanxiaobao.xyz/Article/details/gpbolpvwm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpuczbkps.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gykfpomyz.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxtqjtbkm.sHtML

[S26] C：内存清零
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giduofmqa.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fanxiaobao.xyz/Article/details/gpbxdcisj.sHtML

[S27] C：定义常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gnjsaalrw.sHtML

const double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtlgtrspx.sHtML

[S28] C：静态变量
来源：http://www.share.fanxiaobao.xyz/Article/details/guaiklqbq.sHtML

static int counter = 0;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvyghqyr.sHtML

[S29] C：变参函数
来源：http://blog.fanxiaobao.xyz/Article/details/gbhwbebas.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcjxjvfkl.sHtML

[S30] C：头文件保护
来源：http://blog.fanxiaobao.xyz/Article/details/gezylghpk.sHtML

#ifndef X_H
来源：http://baike.fanxiaobao.xyz/Article/details/gbqyhqdbb.sHtML

#define X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gingfdgvf.sHtML

#endif
来源：http://mobile.fanxiaobao.xyz/Article/details/gqwimisnq.sHtML

[S31] C++：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gwsfzljbe.sHtML

#include <iostream>
来源：http://wap.fanxiaobao.xyz/Article/details/gxtswixtp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/golwcppdy.sHtML

[S32] C++：字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gxhuwtrav.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzeeoezio.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fanxiaobao.xyz/Article/details/geowxkzau.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghndrqqvy.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fanxiaobao.xyz/Article/details/gnoqxdcks.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmajjqddf.sHtML

[S35] C++：map
来源：http://3g.fanxiaobao.xyz/Article/details/gzduzdsgu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gregucvin.sHtML

[S36] C++：unordered_map
来源：http://3g.fanxiaobao.xyz/Article/details/gjctzxjmf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/golpodutb.sHtML

[S37] C++：set
来源：http://mobile.fanxiaobao.xyz/Article/details/gdibubleq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gcvzwhvaj.sHtML

[S38] C++：排序
来源：http://www.share.fanxiaobao.xyz/Article/details/glczvzaae.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gswvhmaeb.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gpnzxvtvc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwcgqhbwq.sHtML

[S40] C++：查找元素
来源：http://baike.fanxiaobao.xyz/Article/details/garhkaeyk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gszaskjom.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyyktclpy.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fanxiaobao.xyz/Article/details/gjolikros.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gfanptfhi.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gokpfkytu.sHtML


<!-- 参考信息 -->