代发 wailian999

[Q82] 字符长度与字节长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gvqiuooum.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gfkbhvquk.sHtML

[Q83] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gcgfsbsmp.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gbjauqvjh.sHtML

[Q84] 去除首尾空格
来源：http://blog.fanxiaobao.xyz/Article/details/guuiuclwr.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcwoiiuvh.sHtML

[Q85] 数值取整
来源：http://mobile.fanxiaobao.xyz/Article/details/gheticfvv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fanxiaobao.xyz/Article/details/gsqvrttie.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fanxiaobao.xyz/Article/details/goymrxcwo.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcwbxmmwu.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fanxiaobao.xyz/Article/details/gjgmrtrbi.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnddyzbpw.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fanxiaobao.xyz/Article/details/gxgpsgzed.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fanxiaobao.xyz/Article/details/gyahpjrqf.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gydzteubk.sHtML

[Q89] 判断表是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gnwfkmhwv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fanxiaobao.xyz/Article/details/gipkuipqd.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtqvsyklx.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaqjbbvwk.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gatugnjvo.sHtML

R. Bash 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gxwpmnkeo.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gvgfztavq.sHtML

[R01] shebang 与严格模式
来源：http://3g.fanxiaobao.xyz/Article/details/gmbejqcub.sHtML

#!/usr/bin/env bash
来源：http://3g.fanxiaobao.xyz/Article/details/gpcdjmtmv.sHtML

set -euo pipefail
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdjqgnfbi.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fanxiaobao.xyz/Article/details/gbbnsayiq.sHtML

name="Tom"; echo "$name"
来源：http://3g.fanxiaobao.xyz/Article/details/gxggzmhki.sHtML

[R03] 只读变量
来源：http://blog.fanxiaobao.xyz/Article/details/gesoazdsy.sHtML

readonly PI=3.14
来源：http://www.share.fanxiaobao.xyz/Article/details/giogdgldq.sHtML

[R04] 位置参数
来源：http://www.share.fanxiaobao.xyz/Article/details/ggerbpqqu.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fanxiaobao.xyz/Article/details/garsevkjj.sHtML

[R05] 参数默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/gpdxmocnt.sHtML

name="${1:-default}"
来源：http://wap.fanxiaobao.xyz/Article/details/gcbcyoljx.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gwbcelwnp.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gobckvkxr.sHtML

[R07] if 判断文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gedoumryg.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxekvyrhm.sHtML

[R08] 数值比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geherfatr.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/guyvpjwgn.sHtML

[R09] 字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gtykzcerr.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gqzndlkpl.sHtML

[R10] 正则匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gmaiooubf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdhxkxmcn.sHtML

[R11] case 多分支
来源：http://m.share.fanxiaobao.xyz/Article/details/ggsolcuaa.sHtML

case "$1" in
来源：http://www.share.fanxiaobao.xyz/Article/details/ggloappyh.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxefugcn.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjpivyqqm.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gidoqytlo.sHtML

esac
来源：http://baike.fanxiaobao.xyz/Article/details/gublzvzme.sHtML

[R12] for 遍历文件
来源：http://3g.fanxiaobao.xyz/Article/details/gprakjgoq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gqojsmaig.sHtML

[R13] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/giowbimjh.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gddyxyjfy.sHtML

[R14] C 风格 for
来源：http://mobile.fanxiaobao.xyz/Article/details/gcbeyfeue.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/govhftauu.sHtML

[R15] while 逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gafyobroh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gowxqsrzr.sHtML

[R16] until 等待条件
来源：http://baike.fanxiaobao.xyz/Article/details/gkelzgaih.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gpwqqraia.sHtML

[R17] 数组定义与取值
来源：http://baike.fanxiaobao.xyz/Article/details/gnuclimnr.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gsnoikvay.sHtML

[R18] 遍历数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gayotamkj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjheewaie.sHtML

[R19] 数组长度
来源：http://blog.fanxiaobao.xyz/Article/details/gpjotovkw.sHtML

echo "${#arr[@]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gunrhoqwn.sHtML

[R20] 关联数组（字典）
来源：http://blog.fanxiaobao.xyz/Article/details/gqfehdhsc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fanxiaobao.xyz/Article/details/ghdsdztmf.sHtML

[R21] 字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gmnmezgbk.sHtML

echo "${#s}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghcphsrrr.sHtML

[R22] 截取子串
来源：http://wap.fanxiaobao.xyz/Article/details/grcplxerj.sHtML

echo "${s:0:5}"
来源：http://blog.fanxiaobao.xyz/Article/details/gkosmowtu.sHtML

[R23] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gtnbctapr.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gvwxjpgjo.sHtML

[R24] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/ggmbasoxr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/gdjlrncxl.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fanxiaobao.xyz/Article/details/gnyycbekm.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbzmtndy.sHtML

[R26] 命令替换
来源：http://blog.fanxiaobao.xyz/Article/details/gywocklpl.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fanxiaobao.xyz/Article/details/ggzuhnyci.sHtML

[R27] 算术展开
来源：http://wap.fanxiaobao.xyz/Article/details/gvcmotjrc.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/gkdlpvfki.sHtML

[R28] 浮点运算
来源：http://baike.fanxiaobao.xyz/Article/details/gudsgmmbf.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fanxiaobao.xyz/Article/details/gglufpgpt.sHtML

[R29] 定义函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gkxjbbyga.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fanxiaobao.xyz/Article/details/glbrulryy.sHtML

[R30] 函数返回状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gckwszdek.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtepnhipb.sHtML

[R31] 局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gucihgsfx.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxfvjmugm.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpuxduokq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gpnhwxfiz.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfydodsft.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fanxiaobao.xyz/Article/details/gavsfxobx.sHtML

[R34] 退出时清理
来源：http://m.share.fanxiaobao.xyz/Article/details/gaicnmven.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gpobhhibo.sHtML

[R35] 后台执行并等待
来源：http://mobile.fanxiaobao.xyz/Article/details/gggqtsvet.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdusgwfwf.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gapnguwbk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchpqjydi.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gbpelxslc.sHtML

files=$(ls -1)
来源：http://3g.fanxiaobao.xyz/Article/details/gqryopqyc.sHtML

[R38] 管道串联
来源：http://blog.fanxiaobao.xyz/Article/details/gtnfnpsjj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnftyzcgs.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gglzgcmxy.sHtML

cmd > out.log 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gztdvbhgt.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghjggbucl.sHtML

echo "log" >> out.log
来源：http://blog.fanxiaobao.xyz/Article/details/gcqpgytfa.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkrisspat.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gftcycspz.sHtML

[R42] 输入重定向
来源：http://3g.fanxiaobao.xyz/Article/details/gfydkurnr.sHtML

wc -l < a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gqpnjrysi.sHtML

[R43] 按名字查找文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gngpyieui.sHtML

find . -name "*.log" -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gvcgikmtj.sHtML

[R44] 按修改时间查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gumjzoyew.sHtML

find . -mtime -7 -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gqejmwvzh.sHtML

[R45] 批量删除
来源：http://read.share.fanxiaobao.xyz/Article/details/goueqoygv.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fanxiaobao.xyz/Article/details/gcfatmnox.sHtML

[R46] 递归替换文件内容
来源：http://wap.fanxiaobao.xyz/Article/details/gixkiwsif.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fanxiaobao.xyz/Article/details/gdzgmuwte.sHtML

[R47] sed 单行替换
来源：http://3g.fanxiaobao.xyz/Article/details/gezvhhnlf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gquxcvzbt.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/gcmxvkydf.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/ggochcebr.sHtML

[R49] awk 带条件
来源：http://3g.fanxiaobao.xyz/Article/details/gcjpltacl.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fanxiaobao.xyz/Article/details/gmartngph.sHtML

[R50] awk 求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gssrddrje.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gimoioxdz.sHtML

[R51] 排序去重取前几
来源：http://blog.fanxiaobao.xyz/Article/details/gutpbjwvm.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fanxiaobao.xyz/Article/details/gukovqbvw.sHtML

[R52] 统计行数
来源：http://www.share.fanxiaobao.xyz/Article/details/glmxcdzxq.sHtML

wc -l a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvfuhnkh.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fanxiaobao.xyz/Article/details/gmyoiufbo.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/grmdlelxm.sHtML

[R54] 比较两个文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gkcrztlat.sHtML

diff a.txt b.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghutnjwmi.sHtML

[R55] 压缩与解压
来源：http://wap.fanxiaobao.xyz/Article/details/gwmtwvszk.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fanxiaobao.xyz/Article/details/gigxixrsl.sHtML

[R56] 远程拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gzrjnujht.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/gceyaridu.sHtML

[R57] 远程执行命令
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsqzhqmha.sHtML

ssh user@host 'uptime'
来源：http://wap.fanxiaobao.xyz/Article/details/gedbxqwmg.sHtML

[R58] 下载文件
来源：http://mobile.fanxiaobao.xyz/Article/details/guahlcgpf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/gyrmimzmb.sHtML

[R59] 发 POST JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gxsauosgl.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gvqvyhypw.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gmjkolefx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdlrrppgy.sHtML

[R61] 磁盘占用
来源：http://baike.fanxiaobao.xyz/Article/details/gmmqzwibg.sHtML

df -h;  du -sh *
来源：http://www.share.fanxiaobao.xyz/Article/details/ghiakzcbb.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gteotvwsq.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fanxiaobao.xyz/Article/details/gagtwqbiw.sHtML

[R63] 内存与进程
来源：http://m.share.fanxiaobao.xyz/Article/details/ggjewqhlh.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fanxiaobao.xyz/Article/details/gcuizknky.sHtML

[R64] 结束进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gtbocvrah.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fanxiaobao.xyz/Article/details/grdfyaikw.sHtML

[R65] 查看端口占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/grwruepmm.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/gipcnizhe.sHtML

[R66] 定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gklrpcogp.sHtML

crontab -e;  crontab -l
来源：http://read.share.fanxiaobao.xyz/Article/details/ghlbxssdk.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fanxiaobao.xyz/Article/details/glohlrwby.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/gpzienfig.sHtML

[R68] 计算文件校验值
来源：http://mobile.fanxiaobao.xyz/Article/details/ghbhlxzce.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gfxhnuehc.sHtML

[R69] 生成随机密码
来源：http://m.share.fanxiaobao.xyz/Article/details/gqabzugee.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fanxiaobao.xyz/Article/details/gjhizyfbd.sHtML

[R70] 时间戳与互转
来源：http://read.share.fanxiaobao.xyz/Article/details/gwgxdgisy.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grgyylwit.sHtML

[R71] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/ggjoytpnh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fanxiaobao.xyz/Article/details/gsygzfrmg.sHtML

[R72] 等待端口就绪
来源：http://3g.fanxiaobao.xyz/Article/details/gyfjihpjk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gnrafnhny.sHtML

[R73] 分割大日志
来源：http://baike.fanxiaobao.xyz/Article/details/gtvkuzmcm.sHtML

split -l 1000 big.log part_
来源：http://wap.fanxiaobao.xyz/Article/details/gcfmuelnr.sHtML

[R74] 批量重命名
来源：http://m.share.fanxiaobao.xyz/Article/details/gansidedz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gbianjymd.sHtML

[R75] 导出环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/glkyntjkr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/gesdlkojb.sHtML

[R76] 使用临时文件
来源：http://3g.fanxiaobao.xyz/Article/details/gxbqzclkb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gdwhqqjmp.sHtML

[R77] 读取用户输入
来源：http://m.share.fanxiaobao.xyz/Article/details/gliffnyan.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzonclxuw.sHtML

[R78] 交互式菜单
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfpsarvrp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gtnsrhtuo.sHtML

[R79] 解析命令行选项
来源：http://baike.fanxiaobao.xyz/Article/details/gckyhrlvy.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gxcifzjnx.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmtmxhefa.sHtML

time ./run.sh
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtdoqvesn.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gsgysldpw.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gsjiwzkiw.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gcdiocxcr.sHtML

[S01] C：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gqgbnpivg.sHtML

#include <stdio.h>
来源：http://baike.fanxiaobao.xyz/Article/details/gquxtvxlw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fanxiaobao.xyz/Article/details/gtqsxpozw.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fanxiaobao.xyz/Article/details/grxnxtsmt.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fanxiaobao.xyz/Article/details/gtjolqvpl.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gbhcwbkoq.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggdsuyexh.sHtML

[S04] C：字符串复制
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbwmnmzx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fanxiaobao.xyz/Article/details/gebiiopyn.sHtML

[S05] C：字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggvmnlmln.sHtML

strlen(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvyydvhf.sHtML

[S06] C：字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gzcerfzcu.sHtML

strcmp(a, b) == 0
来源：http://www.share.fanxiaobao.xyz/Article/details/gsdmgyfpo.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaheegtfx.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fanxiaobao.xyz/Article/details/gbximqjcs.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gouwumhwu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxqflssvc.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbuojpum.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmnymbmrn.sHtML

[S10] C：指针与解引用
来源：http://wap.fanxiaobao.xyz/Article/details/gdyvnqvyn.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fanxiaobao.xyz/Article/details/gddraztfj.sHtML

[S11] C：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gqqwqdlyo.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvzsqesf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gtqbbrluv.sHtML

fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gdwwvkivt.sHtML

[S12] C：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/glfovzxgm.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gcsdznikq.sHtML

[S13] C：宏定义
来源：http://3g.fanxiaobao.xyz/Article/details/gdrapohww.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fanxiaobao.xyz/Article/details/grfdeqnjh.sHtML

[S14] C：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gggyojxhp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fanxiaobao.xyz/Article/details/gtnnfhalc.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gqldauhca.sHtML

(double) a / b
来源：http://3g.fanxiaobao.xyz/Article/details/gbromdnoq.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggkhrxbob.sHtML

x |= (1 << 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gpohacwgv.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gzeeepvvn.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fanxiaobao.xyz/Article/details/geftsbkks.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyknwfpcq.sHtML

int main(int argc, char **argv)
来源：http://blog.fanxiaobao.xyz/Article/details/gubjchctq.sHtML

[S19] C：快速排序
来源：http://baike.fanxiaobao.xyz/Article/details/guhlainkv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gsifrvdot.sHtML

[S20] C：二分查找
来源：http://baike.fanxiaobao.xyz/Article/details/gmgijyssk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gnlhmakik.sHtML

[S21] C：字符类别判断
来源：http://blog.fanxiaobao.xyz/Article/details/gnrvyvupl.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghzydpjdo.sHtML

[S22] C：字符串转数字
来源：http://3g.fanxiaobao.xyz/Article/details/gzgirvysl.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdshcrmcf.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/gtpfbsjkr.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gmimcofta.sHtML

[S24] C：获取本地时间
来源：http://baike.fanxiaobao.xyz/Article/details/gzoeugkkv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkaitnsqx.sHtML

[S25] C：内存拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/grvhrdido.sHtML

memcpy(dst, src, n);
来源：http://baike.fanxiaobao.xyz/Article/details/getsxvbbd.sHtML

[S26] C：内存清零
来源：http://baike.fanxiaobao.xyz/Article/details/gkwnnaacw.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fanxiaobao.xyz/Article/details/gabbsszpl.sHtML

[S27] C：定义常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gzlxfcdxz.sHtML

const double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkzqwsplx.sHtML

[S28] C：静态变量
来源：http://wap.fanxiaobao.xyz/Article/details/gspamquvl.sHtML

static int counter = 0;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqekmdfxf.sHtML

[S29] C：变参函数
来源：http://baike.fanxiaobao.xyz/Article/details/gaicbwjjh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fanxiaobao.xyz/Article/details/gvrfkhwwl.sHtML

[S30] C：头文件保护
来源：http://wap.fanxiaobao.xyz/Article/details/gkamkcdly.sHtML

#ifndef X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gzqygbevf.sHtML

#define X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gufomoyto.sHtML

#endif
来源：http://baike.fanxiaobao.xyz/Article/details/gibludsag.sHtML

[S31] C++：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gqzpsseml.sHtML

#include <iostream>
来源：http://blog.fanxiaobao.xyz/Article/details/glomyfouj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gshhrbwmi.sHtML

[S32] C++：字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glmhzytua.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyqmboets.sHtML

[S33] C++：vector 增删
来源：http://blog.fanxiaobao.xyz/Article/details/gpmvhhzkz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gbmlocxxz.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fanxiaobao.xyz/Article/details/gzykaxhgm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gupepxjvk.sHtML

[S35] C++：map
来源：http://baike.fanxiaobao.xyz/Article/details/gplphmrkz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbtctpvcr.sHtML

[S36] C++：unordered_map
来源：http://mobile.fanxiaobao.xyz/Article/details/gfusxuonc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqkwlfdya.sHtML

[S37] C++：set
来源：http://blog.fanxiaobao.xyz/Article/details/ghxnpwdgl.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gqzhytyqd.sHtML

[S38] C++：排序
来源：http://3g.fanxiaobao.xyz/Article/details/gvcxjpdnk.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/grtwkbdct.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fanxiaobao.xyz/Article/details/gxcljdkcn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fanxiaobao.xyz/Article/details/gjspdyrqt.sHtML

[S40] C++：查找元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtvjwkgxm.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gewvllwyg.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fanxiaobao.xyz/Article/details/grfqpbiwt.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmzanpkzw.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fanxiaobao.xyz/Article/details/giyxhquyo.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fanxiaobao.xyz/Article/details/gatrspvlr.sHtML

[S43] C++：智能指针
来源：http://wap.fanxiaobao.xyz/Article/details/gnhgxdjwq.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvapzmmvk.sHtML

[S44] C++：引用传参
来源：http://www.blog.fanxiaobao.xyz/Article/details/guomqdbil.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gbrxzwdet.sHtML

[S45] C++：lambda
来源：http://blog.fanxiaobao.xyz/Article/details/gbjkuqask.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gkunjvaqw.sHtML

[S46] C++：函数模板
来源：http://3g.fanxiaobao.xyz/Article/details/gmossnyjb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggeyzbovt.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyqrewwnm.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbgjyncg.sHtML

[S48] C++：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gdvaquhyq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fanxiaobao.xyz/Article/details/gaktwyxsd.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gytedxhbl.sHtML

[S49] C++：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/glebwfuss.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gnfoxyxwq.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjomdnwj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gusekuxzp.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjjooxlcp.sHtML

static_cast<double>(a) / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gkwgmqxnc.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fanxiaobao.xyz/Article/details/glvncvmeu.sHtML


<!-- 参考信息 -->