代发 wailian999

[Q80] 字符串截取
来源：http://m.share.fanxiaobao.xyz/Article/details/gjdmmdiqh.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghxzfeaqu.sHtML

[Q81] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvnfpbul.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/ggucunlae.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fanxiaobao.xyz/Article/details/gfkbhfovz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzylavsbh.sHtML

[Q83] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gipohklwx.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjwbuxrrd.sHtML

[Q84] 去除首尾空格
来源：http://baike.fanxiaobao.xyz/Article/details/gciuwiivs.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gmgmmdwnw.sHtML

[Q85] 数值取整
来源：http://wap.fanxiaobao.xyz/Article/details/gsxginndy.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fanxiaobao.xyz/Article/details/guuwxrzvy.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxugntzos.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjvexnxih.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjzptsxrh.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fanxiaobao.xyz/Article/details/gefhpuule.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fanxiaobao.xyz/Article/details/gxxvnldvj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fanxiaobao.xyz/Article/details/gqhahumye.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajywszhg.sHtML

[Q89] 判断表是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gtvkxkfda.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/gmfngvvsb.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcexaoubc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gthxtbxdo.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gbpaovbek.sHtML

R. Bash 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gcqkshwbu.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnzmuqmzn.sHtML

[R01] shebang 与严格模式
来源：http://3g.fanxiaobao.xyz/Article/details/gcouyzgpr.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fanxiaobao.xyz/Article/details/gocfhbtef.sHtML

set -euo pipefail
来源：http://www.blog.fanxiaobao.xyz/Article/details/gahwhfdet.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwmbuepjx.sHtML

name="Tom"; echo "$name"
来源：http://wap.fanxiaobao.xyz/Article/details/gozsiwuyc.sHtML

[R03] 只读变量
来源：http://wap.fanxiaobao.xyz/Article/details/grhkqrvgi.sHtML

readonly PI=3.14
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghxnklyga.sHtML

[R04] 位置参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gptrbunsp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fanxiaobao.xyz/Article/details/ghreznuol.sHtML

[R05] 参数默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/gquyflwca.sHtML

name="${1:-default}"
来源：http://read.share.fanxiaobao.xyz/Article/details/griitlpyt.sHtML

[R06] 判断命令是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gxpowbnvo.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/guxtzyits.sHtML

[R07] if 判断文件
来源：http://wap.fanxiaobao.xyz/Article/details/gdsqzqgay.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gfniuvpxc.sHtML

[R08] 数值比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfnvoppwj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gawknfxuh.sHtML

[R09] 字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gyybigftl.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gxtbhdvss.sHtML

[R10] 正则匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gfcgfuebo.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gqvlexcaj.sHtML

[R11] case 多分支
来源：http://read.share.fanxiaobao.xyz/Article/details/gcgelvgup.sHtML

case "$1" in
来源：http://wap.fanxiaobao.xyz/Article/details/gmyeszujd.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqkcljbd.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/genxwtxte.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/ggbylpujv.sHtML

esac
来源：http://mobile.fanxiaobao.xyz/Article/details/gjvltifzd.sHtML

[R12] for 遍历文件
来源：http://wap.fanxiaobao.xyz/Article/details/gqksxfryl.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geglgoxpm.sHtML

[R13] for 计数循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gaelktdxh.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gedwtpkkn.sHtML

[R14] C 风格 for
来源：http://wap.fanxiaobao.xyz/Article/details/gqkioywok.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywrqdchw.sHtML

[R15] while 逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/ghgxriojv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gweoymfrq.sHtML

[R16] until 等待条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gyiodubps.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gbpujwvns.sHtML

[R17] 数组定义与取值
来源：http://read.share.fanxiaobao.xyz/Article/details/gveuhewqp.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjqcyushg.sHtML

[R18] 遍历数组
来源：http://3g.fanxiaobao.xyz/Article/details/grqucnpnx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gdqcsyued.sHtML

[R19] 数组长度
来源：http://read.share.fanxiaobao.xyz/Article/details/glqwwlftc.sHtML

echo "${#arr[@]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gwxroggup.sHtML

[R20] 关联数组（字典）
来源：http://3g.fanxiaobao.xyz/Article/details/gmzufbavv.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gxqfmhfmf.sHtML

[R21] 字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqbrfotxk.sHtML

echo "${#s}"
来源：http://baike.fanxiaobao.xyz/Article/details/gpdyggmuu.sHtML

[R22] 截取子串
来源：http://read.share.fanxiaobao.xyz/Article/details/gffgoqulh.sHtML

echo "${s:0:5}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtoyxhovt.sHtML

[R23] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gzpufagpx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gasusllst.sHtML

[R24] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gagjsdjaw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fanxiaobao.xyz/Article/details/ghixiiefj.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fanxiaobao.xyz/Article/details/gybgnyzia.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gvvgazxjh.sHtML

[R26] 命令替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gbmetywsx.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fanxiaobao.xyz/Article/details/gfzcztdbg.sHtML

[R27] 算术展开
来源：http://3g.fanxiaobao.xyz/Article/details/gtvbuozbw.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/gdxdivbmz.sHtML

[R28] 浮点运算
来源：http://3g.fanxiaobao.xyz/Article/details/gypapcnxc.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fanxiaobao.xyz/Article/details/gjqyrwssc.sHtML

[R29] 定义函数
来源：http://mobile.fanxiaobao.xyz/Article/details/getyejqxs.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gsatiqjzy.sHtML

[R30] 函数返回状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gutsirejc.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fanxiaobao.xyz/Article/details/gbwsntmrz.sHtML

[R31] 局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gnsnqjwqw.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gytuylflp.sHtML

[R32] 参数个数校验
来源：http://www.share.fanxiaobao.xyz/Article/details/gnumarblb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gdekndjgx.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fanxiaobao.xyz/Article/details/gcidtficp.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggwtzhkwk.sHtML

[R34] 退出时清理
来源：http://3g.fanxiaobao.xyz/Article/details/gylpgmtwy.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gxbmoenrz.sHtML

[R35] 后台执行并等待
来源：http://baike.fanxiaobao.xyz/Article/details/gkatyntva.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fanxiaobao.xyz/Article/details/gblabwkcw.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfxuqiahh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fanxiaobao.xyz/Article/details/gadypegmc.sHtML

[R37] 把输出赋给变量
来源：http://wap.fanxiaobao.xyz/Article/details/grmpzlabh.sHtML

files=$(ls -1)
来源：http://mobile.fanxiaobao.xyz/Article/details/galvdncaj.sHtML

[R38] 管道串联
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdaklnof.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gqnzphpqt.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fanxiaobao.xyz/Article/details/gznvuxieq.sHtML

cmd > out.log 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gkcgefahj.sHtML

[R40] 追加写日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gqaxgelch.sHtML

echo "log" >> out.log
来源：http://baike.fanxiaobao.xyz/Article/details/gpqrxtwqo.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqgckzpme.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/grwndogcq.sHtML

[R42] 输入重定向
来源：http://mobile.fanxiaobao.xyz/Article/details/gcnctoowv.sHtML

wc -l < a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/ghaouvjqk.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/glpssnnod.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glaelbaks.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gknjkfrnv.sHtML

find . -mtime -7 -type f
来源：http://blog.fanxiaobao.xyz/Article/details/ghoocloen.sHtML

[R45] 批量删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevnfeqfu.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fanxiaobao.xyz/Article/details/gvxihkwwf.sHtML

[R46] 递归替换文件内容
来源：http://wap.fanxiaobao.xyz/Article/details/gnolrvwzu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzxmxxjoc.sHtML

[R47] sed 单行替换
来源：http://wap.fanxiaobao.xyz/Article/details/gsjrvndkq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/guxgsmotj.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gvudgljan.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/grjyudyeh.sHtML

[R49] awk 带条件
来源：http://3g.fanxiaobao.xyz/Article/details/glmyvxfzb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fanxiaobao.xyz/Article/details/gjklgbmqo.sHtML

[R50] awk 求和
来源：http://3g.fanxiaobao.xyz/Article/details/gqoockbur.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gepmwcyll.sHtML

[R51] 排序去重取前几
来源：http://3g.fanxiaobao.xyz/Article/details/gpahplbpt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fanxiaobao.xyz/Article/details/gqvgeuqki.sHtML

[R52] 统计行数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gybclausl.sHtML

wc -l a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gfgzahwiz.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fanxiaobao.xyz/Article/details/gubwjhouj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glykftkci.sHtML

[R54] 比较两个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gfnpxclny.sHtML

diff a.txt b.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gxlpdgmiq.sHtML

[R55] 压缩与解压
来源：http://baike.fanxiaobao.xyz/Article/details/gyrnqejyv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fanxiaobao.xyz/Article/details/gwvqrwcjl.sHtML

[R56] 远程拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/ghyoaskqh.sHtML

scp file user@host:/path/
来源：http://m.share.fanxiaobao.xyz/Article/details/gqqaqccdd.sHtML

[R57] 远程执行命令
来源：http://baike.fanxiaobao.xyz/Article/details/gzrubtnum.sHtML

ssh user@host 'uptime'
来源：http://baike.fanxiaobao.xyz/Article/details/gwtowrglh.sHtML

[R58] 下载文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gvxnwaeym.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fanxiaobao.xyz/Article/details/gvrdcxrmx.sHtML

[R59] 发 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/gccdumhsi.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fanxiaobao.xyz/Article/details/gvbocuwis.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gpoasulyo.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fanxiaobao.xyz/Article/details/gfmboflfe.sHtML

[R61] 磁盘占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gqyuzgcux.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/gxgmktcdx.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fanxiaobao.xyz/Article/details/ghrmkmtpd.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fanxiaobao.xyz/Article/details/gtjffauct.sHtML

[R63] 内存与进程
来源：http://wap.fanxiaobao.xyz/Article/details/guwujjfwj.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fanxiaobao.xyz/Article/details/gyscxmfbr.sHtML

[R64] 结束进程
来源：http://wap.fanxiaobao.xyz/Article/details/gllacqxgr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fanxiaobao.xyz/Article/details/getzdzbio.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbswveyw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fanxiaobao.xyz/Article/details/gdcrujowx.sHtML

[R66] 定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gtotcgcef.sHtML

crontab -e;  crontab -l
来源：http://3g.fanxiaobao.xyz/Article/details/gfkpxuepr.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkrideuit.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/gzgxaninz.sHtML

[R68] 计算文件校验值
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhkpfyhl.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gtstlkupi.sHtML

[R69] 生成随机密码
来源：http://wap.fanxiaobao.xyz/Article/details/gatvqueex.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fanxiaobao.xyz/Article/details/gmjkmiuod.sHtML

[R70] 时间戳与互转
来源：http://mobile.fanxiaobao.xyz/Article/details/gsljfyvzl.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fanxiaobao.xyz/Article/details/gwracjfrk.sHtML

[R71] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gnzdfdfxp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fanxiaobao.xyz/Article/details/gcodjukba.sHtML

[R72] 等待端口就绪
来源：http://baike.fanxiaobao.xyz/Article/details/gpzyomeob.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggzyepcsz.sHtML

[R73] 分割大日志
来源：http://blog.fanxiaobao.xyz/Article/details/gwyycxcbn.sHtML

split -l 1000 big.log part_
来源：http://read.share.fanxiaobao.xyz/Article/details/glkfbfagr.sHtML

[R74] 批量重命名
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxovlybmr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gbuvrtcai.sHtML

[R75] 导出环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gqzwrjjnh.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fanxiaobao.xyz/Article/details/ghtsgpzgs.sHtML

[R76] 使用临时文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gkuevzbya.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gwxsttqrx.sHtML

[R77] 读取用户输入
来源：http://wap.fanxiaobao.xyz/Article/details/gpsemdimc.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gitimzcdm.sHtML

[R78] 交互式菜单
来源：http://blog.fanxiaobao.xyz/Article/details/gskznfart.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gecobbrkh.sHtML

[R79] 解析命令行选项
来源：http://3g.fanxiaobao.xyz/Article/details/gqrdzdrcd.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gyitvojts.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fanxiaobao.xyz/Article/details/gagbjxsfa.sHtML

time ./run.sh
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzmrdlgig.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gkmewnxby.sHtML

S. C / C++ 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/guywpwyya.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gbhubukfu.sHtML

[S01] C：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gofgtdqct.sHtML

#include <stdio.h>
来源：http://read.share.fanxiaobao.xyz/Article/details/gwfldhvpk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gijnzakpy.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/glevrhbxd.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fanxiaobao.xyz/Article/details/gwokxbysj.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gsfpgfprj.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfbrzxtvv.sHtML

[S04] C：字符串复制
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjkutvmb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fanxiaobao.xyz/Article/details/gwyyspisv.sHtML

[S05] C：字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gandpxvbg.sHtML

strlen(s)
来源：http://baike.fanxiaobao.xyz/Article/details/grswrarwp.sHtML

[S06] C：字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gpanhvjht.sHtML

strcmp(a, b) == 0
来源：http://blog.fanxiaobao.xyz/Article/details/gbeqbygnu.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gntoneyjs.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fanxiaobao.xyz/Article/details/geqpvflme.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshrwrlcs.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqjjxiqji.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fanxiaobao.xyz/Article/details/gcnbzcngp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fanxiaobao.xyz/Article/details/gwwtgnwbr.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grvgwgfmu.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqwtsuaeo.sHtML

[S11] C：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gmbxcycwq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghfckbjsc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnkcxgyaq.sHtML

fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdisbcbhb.sHtML

[S12] C：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gabgzexti.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gjlssxjye.sHtML

[S13] C：宏定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gdjfaweoi.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fanxiaobao.xyz/Article/details/gnxyjwlxh.sHtML

[S14] C：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/glvpzufga.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fanxiaobao.xyz/Article/details/gndmkfcrb.sHtML

[S15] C：类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gcvcgvvwx.sHtML

(double) a / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyfroizxp.sHtML

[S16] C：位操作置位
来源：http://www.blog.fanxiaobao.xyz/Article/details/glfkdrbjm.sHtML

x |= (1 << 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/goalomwbf.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gzlshsxbw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmwwvkowu.sHtML

[S18] C：命令行参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/glsddqtid.sHtML

int main(int argc, char **argv)
来源：http://m.share.fanxiaobao.xyz/Article/details/gazeppgdd.sHtML

[S19] C：快速排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gdpqudgjq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gmntfkdyh.sHtML

[S20] C：二分查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gwkumidtx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gikhsjhlb.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grexstkfk.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfixvgnhy.sHtML

[S22] C：字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gewhlzepz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxvsbwcyx.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/gyiaaghta.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxthmwipk.sHtML

[S24] C：获取本地时间
来源：http://www.share.fanxiaobao.xyz/Article/details/goekxdhnq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fanxiaobao.xyz/Article/details/grbyrvzfl.sHtML

[S25] C：内存拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gupupqxey.sHtML

memcpy(dst, src, n);
来源：http://3g.fanxiaobao.xyz/Article/details/guybalkei.sHtML

[S26] C：内存清零
来源：http://www.share.fanxiaobao.xyz/Article/details/gwlyjihqb.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gokrjuxig.sHtML

[S27] C：定义常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfodjspvy.sHtML

const double PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gdpzstnex.sHtML

[S28] C：静态变量
来源：http://mobile.fanxiaobao.xyz/Article/details/guiaeevyv.sHtML

static int counter = 0;
来源：http://baike.fanxiaobao.xyz/Article/details/goetmazcu.sHtML

[S29] C：变参函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gcsmnnnhu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fanxiaobao.xyz/Article/details/gqluptktw.sHtML

[S30] C：头文件保护
来源：http://m.share.fanxiaobao.xyz/Article/details/gqfflhmjd.sHtML

#ifndef X_H
来源：http://3g.fanxiaobao.xyz/Article/details/guhclmuda.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfqxeztp.sHtML

#endif
来源：http://wap.fanxiaobao.xyz/Article/details/guayqaote.sHtML

[S31] C++：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/grhzzxnrm.sHtML

#include <iostream>
来源：http://blog.fanxiaobao.xyz/Article/details/gjqwmskte.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjfewllwq.sHtML

[S32] C++：字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gfvaxwbeb.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyixbfdli.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpvzabpbc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gqfrxqbcc.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqsazkgz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghnraygkm.sHtML

[S35] C++：map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbnqrxlmy.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/grtiulwuz.sHtML

[S36] C++：unordered_map
来源：http://baike.fanxiaobao.xyz/Article/details/gpwnduvov.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gtuvmdwfd.sHtML

[S37] C++：set
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkyqgrdvq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/grscbgjiw.sHtML

[S38] C++：排序
来源：http://wap.fanxiaobao.xyz/Article/details/gubjcsfpr.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gjwtxthwl.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fanxiaobao.xyz/Article/details/gywjyjitr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fanxiaobao.xyz/Article/details/gahbmyinc.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gbhgkodpo.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/grsneetis.sHtML

[S41] C++：类与构造函数
来源：http://wap.fanxiaobao.xyz/Article/details/gshcylafc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdowbgraa.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpezqeeys.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fanxiaobao.xyz/Article/details/guklzdkfd.sHtML

[S43] C++：智能指针
来源：http://m.share.fanxiaobao.xyz/Article/details/gagyujvme.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fanxiaobao.xyz/Article/details/gndrxbsos.sHtML

[S44] C++：引用传参
来源：http://read.share.fanxiaobao.xyz/Article/details/gljimptyu.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzctbkxsk.sHtML

[S45] C++：lambda
来源：http://3g.fanxiaobao.xyz/Article/details/gqgsdfnzr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gbtjfwere.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmqdwuqs.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gxqvmsggc.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/genygjsla.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gupbabipo.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkknrozgh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gclslbyut.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gajsyyzda.sHtML

[S49] C++：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjrtsvbzz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goijepycg.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gezlatfab.sHtML


<!-- 参考信息 -->