代发 wailian999

[Q84] 去除首尾空格
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmaonfbux.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gfkrmtxlx.sHtML

[Q85] 数值取整
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyooizjin.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fanxiaobao.xyz/Article/details/gdyknptya.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fanxiaobao.xyz/Article/details/glvvuyizi.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fanxiaobao.xyz/Article/details/gatazrxrg.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fanxiaobao.xyz/Article/details/gzsyqtqbb.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fanxiaobao.xyz/Article/details/grnkudtux.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvtpcvfee.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fanxiaobao.xyz/Article/details/giejdpupg.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gmazlkggf.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvpyvkeop.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/geomwjeld.sHtML

[Q90] 生成序号列
来源：http://www.share.fanxiaobao.xyz/Article/details/geatpbqdv.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fanxiaobao.xyz/Article/details/geixnttjv.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gzijwidng.sHtML

R. Bash 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gyozwokmc.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gpxjlbryk.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvwlkfjk.sHtML

#!/usr/bin/env bash
来源：http://m.share.fanxiaobao.xyz/Article/details/gejkstuzr.sHtML

set -euo pipefail
来源：http://3g.fanxiaobao.xyz/Article/details/gmfqiwwwy.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fanxiaobao.xyz/Article/details/givszzdri.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbrfygubr.sHtML

[R03] 只读变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmursrvii.sHtML

readonly PI=3.14
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijakynpl.sHtML

[R04] 位置参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gtwrnlrbq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fanxiaobao.xyz/Article/details/gcyqnncpt.sHtML

[R05] 参数默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/gnuzrbbyg.sHtML

name="${1:-default}"
来源：http://m.share.fanxiaobao.xyz/Article/details/grczjddxv.sHtML

[R06] 判断命令是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gficihhip.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcgnfjdcz.sHtML

[R07] if 判断文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmmysmyqv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gepgwpsrq.sHtML

[R08] 数值比较
来源：http://baike.fanxiaobao.xyz/Article/details/gfwgzjrxs.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gswwtdfyl.sHtML

[R09] 字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gaireuupr.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gebkbuxux.sHtML

[R10] 正则匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyojhjvzs.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gmtibbrwl.sHtML

[R11] case 多分支
来源：http://3g.fanxiaobao.xyz/Article/details/gmwlokizj.sHtML

case "$1" in
来源：http://3g.fanxiaobao.xyz/Article/details/gaxjovntx.sHtML

start) echo "启动" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/grtfmouiy.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbaxopbhg.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gaqjhjkzd.sHtML

esac
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggmxnhdvh.sHtML

[R12] for 遍历文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gnlmhkahy.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gkgkieeie.sHtML

[R13] for 计数循环
来源：http://wap.fanxiaobao.xyz/Article/details/ghfxurpbg.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/glykffbsp.sHtML

[R14] C 风格 for
来源：http://3g.fanxiaobao.xyz/Article/details/gldgjrplr.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gpjgmpagj.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjmyugjz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fanxiaobao.xyz/Article/details/ggnddtgcp.sHtML

[R16] until 等待条件
来源：http://3g.fanxiaobao.xyz/Article/details/gfpkvdjxl.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/grqdiaqsz.sHtML

[R17] 数组定义与取值
来源：http://baike.fanxiaobao.xyz/Article/details/gyyazqizs.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gsaxighdj.sHtML

[R18] 遍历数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gzptawrnk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gtrqofehw.sHtML

[R19] 数组长度
来源：http://blog.fanxiaobao.xyz/Article/details/gppqixtwx.sHtML

echo "${#arr[@]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gpxvrapmd.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fanxiaobao.xyz/Article/details/gajqquktc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fanxiaobao.xyz/Article/details/glauojsja.sHtML

[R21] 字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/glncklvhp.sHtML

echo "${#s}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gipmvravc.sHtML

[R22] 截取子串
来源：http://www.share.fanxiaobao.xyz/Article/details/gkudctgxd.sHtML

echo "${s:0:5}"
来源：http://3g.fanxiaobao.xyz/Article/details/gefdqyrht.sHtML

[R23] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gcsjgvpox.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fanxiaobao.xyz/Article/details/ghayznrjt.sHtML

[R24] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggxpzfxfl.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjihvlkg.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fanxiaobao.xyz/Article/details/gtvvyslvj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gekjfjqpz.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gssmsnhap.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fanxiaobao.xyz/Article/details/gfnqbpuek.sHtML

[R27] 算术展开
来源：http://wap.fanxiaobao.xyz/Article/details/gcyhbniso.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fanxiaobao.xyz/Article/details/gwstycext.sHtML

[R28] 浮点运算
来源：http://read.share.fanxiaobao.xyz/Article/details/galbjnabe.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fanxiaobao.xyz/Article/details/gytqtjfzd.sHtML

[R29] 定义函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbpownnxt.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gnflwiofe.sHtML

[R30] 函数返回状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gihxyejbk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fanxiaobao.xyz/Article/details/gyhfdviau.sHtML

[R31] 局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/grlyidepi.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gsjimylrs.sHtML

[R32] 参数个数校验
来源：http://blog.fanxiaobao.xyz/Article/details/gsmhxzzsq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gutlclten.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fanxiaobao.xyz/Article/details/gobwozdoj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fanxiaobao.xyz/Article/details/gubdjunxb.sHtML

[R34] 退出时清理
来源：http://baike.fanxiaobao.xyz/Article/details/gchtqrvtl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpdqtamkz.sHtML

[R35] 后台执行并等待
来源：http://mobile.fanxiaobao.xyz/Article/details/gewhxjggs.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fanxiaobao.xyz/Article/details/giigkkotd.sHtML

[R36] 并发执行多个任务
来源：http://3g.fanxiaobao.xyz/Article/details/ghdwomfoh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fanxiaobao.xyz/Article/details/genpfbcyz.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gubfoopfp.sHtML

files=$(ls -1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbwnoznqf.sHtML

[R38] 管道串联
来源：http://read.share.fanxiaobao.xyz/Article/details/gcnyfadfl.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbuenbfa.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fanxiaobao.xyz/Article/details/galwvxtjf.sHtML

cmd > out.log 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/ghxtlaqrg.sHtML

[R40] 追加写日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gxvviklwk.sHtML

echo "log" >> out.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gnwehpffx.sHtML

[R41] 丢弃输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/giwntjqku.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gytilizfh.sHtML

[R42] 输入重定向
来源：http://www.share.fanxiaobao.xyz/Article/details/gkncztlrg.sHtML

wc -l < a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/graypzppg.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjeiivngt.sHtML

find . -name "*.log" -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gryzngbyv.sHtML

[R44] 按修改时间查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gqkgeujpf.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsxzbsyzj.sHtML

[R45] 批量删除
来源：http://www.share.fanxiaobao.xyz/Article/details/gtmydyhpd.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fanxiaobao.xyz/Article/details/glsslynwf.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fanxiaobao.xyz/Article/details/gncynkgye.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/glnraedxi.sHtML

[R47] sed 单行替换
来源：http://m.share.fanxiaobao.xyz/Article/details/ghkyvfpqg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gflxfxywg.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnhktobev.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gjryqfpku.sHtML

[R49] awk 带条件
来源：http://3g.fanxiaobao.xyz/Article/details/gpkrfchyd.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fanxiaobao.xyz/Article/details/gajuiqsji.sHtML

[R50] awk 求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvpukvrga.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gisqxrssd.sHtML

[R51] 排序去重取前几
来源：http://baike.fanxiaobao.xyz/Article/details/grwwabcdf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxdqqluzj.sHtML

[R52] 统计行数
来源：http://m.share.fanxiaobao.xyz/Article/details/gkfpkygdu.sHtML

wc -l a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzfvgynpf.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/gvwktxryp.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gaypuvmry.sHtML

[R54] 比较两个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gwodrzizy.sHtML

diff a.txt b.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gfpsynhsr.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqaaxvgbk.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggvfgeqiq.sHtML

[R56] 远程拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gjvhhkndi.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/grbdaykwu.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/gwyiwxanm.sHtML

ssh user@host 'uptime'
来源：http://read.share.fanxiaobao.xyz/Article/details/gcmaanvpt.sHtML

[R58] 下载文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gocvhksmc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fanxiaobao.xyz/Article/details/gmabcvfsz.sHtML

[R59] 发 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/gaqadnuvo.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fanxiaobao.xyz/Article/details/gorcgrysh.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gdngdwezw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcykxbruc.sHtML

[R61] 磁盘占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvtvprwe.sHtML

df -h;  du -sh *
来源：http://baike.fanxiaobao.xyz/Article/details/girgugydt.sHtML

[R62] 找最占空间的文件
来源：http://3g.fanxiaobao.xyz/Article/details/gfpxsuwpl.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fanxiaobao.xyz/Article/details/gcldkroez.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gjlurqcqt.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fanxiaobao.xyz/Article/details/gcclkueeu.sHtML

[R64] 结束进程
来源：http://blog.fanxiaobao.xyz/Article/details/giikbzsiv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbnuugpol.sHtML

[R65] 查看端口占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gcakbapjj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/gjikuwkkw.sHtML

[R66] 定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcvejilvo.sHtML

crontab -e;  crontab -l
来源：http://wap.fanxiaobao.xyz/Article/details/ghbnsuxzp.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fanxiaobao.xyz/Article/details/gjnhzjhbq.sHtML

openssl rand -hex 16
来源：http://baike.fanxiaobao.xyz/Article/details/gyuyvjfki.sHtML

[R68] 计算文件校验值
来源：http://m.share.fanxiaobao.xyz/Article/details/gnnxwmqqn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gqgbnkusd.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyznbuqgw.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/gtcnhvoeo.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fanxiaobao.xyz/Article/details/gujzhhgba.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/gorhfruvx.sHtML

[R71] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gjchkmkge.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fanxiaobao.xyz/Article/details/gamftvmue.sHtML

[R72] 等待端口就绪
来源：http://wap.fanxiaobao.xyz/Article/details/grjzdnmav.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gkcazahfg.sHtML

[R73] 分割大日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbkrgwjbm.sHtML

split -l 1000 big.log part_
来源：http://mobile.fanxiaobao.xyz/Article/details/gwaiomzxk.sHtML

[R74] 批量重命名
来源：http://read.share.fanxiaobao.xyz/Article/details/gqcavhodd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gnpbslmqb.sHtML

[R75] 导出环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/glwzgsmwq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpvlvrgmm.sHtML

[R76] 使用临时文件
来源：http://3g.fanxiaobao.xyz/Article/details/gqxtjlbjp.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/ghjlylqfx.sHtML

[R77] 读取用户输入
来源：http://mobile.fanxiaobao.xyz/Article/details/guawgpbnl.sHtML

read -rp "请输入: " ans
来源：http://www.share.fanxiaobao.xyz/Article/details/gbyfuahdy.sHtML

[R78] 交互式菜单
来源：http://baike.fanxiaobao.xyz/Article/details/gpgtnxwxp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fanxiaobao.xyz/Article/details/gziddxpwz.sHtML

[R79] 解析命令行选项
来源：http://3g.fanxiaobao.xyz/Article/details/gfjaysscu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhbqcjvj.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjnijnnh.sHtML

time ./run.sh
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtpqwskpx.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gexwuztgt.sHtML

S. C / C++ 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gfiynrxbi.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gfrhxgmjf.sHtML

[S01] C：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/galzvwqqg.sHtML

#include <stdio.h>
来源：http://wap.fanxiaobao.xyz/Article/details/gapeejgae.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fanxiaobao.xyz/Article/details/guvauerrj.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkqgnozlu.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggmtyilmj.sHtML

[S03] C：读入整数
来源：http://blog.fanxiaobao.xyz/Article/details/gasxeatki.sHtML

int x; scanf("%d", &x);
来源：http://wap.fanxiaobao.xyz/Article/details/gpausvdqm.sHtML

[S04] C：字符串复制
来源：http://mobile.fanxiaobao.xyz/Article/details/gfqsyschs.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gelothytz.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gkugkudbo.sHtML

strlen(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggrchmexl.sHtML

[S06] C：字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gqcbtxevo.sHtML

strcmp(a, b) == 0
来源：http://blog.fanxiaobao.xyz/Article/details/gyzvhhcyj.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/gfbqmxqkt.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fanxiaobao.xyz/Article/details/gmtjixlre.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/gvjnlkfof.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fanxiaobao.xyz/Article/details/gloknfpkz.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fanxiaobao.xyz/Article/details/gzgtimqrj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fanxiaobao.xyz/Article/details/gdefxpixy.sHtML

[S10] C：指针与解引用
来源：http://wap.fanxiaobao.xyz/Article/details/gfzubzirn.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghxhusykk.sHtML

[S11] C：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gwnctdgtt.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxuqgsavo.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxpesdopz.sHtML

fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gedzwielk.sHtML

[S12] C：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gwsztfbrs.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbgtotljd.sHtML

[S13] C：宏定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gttfhxcqw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fanxiaobao.xyz/Article/details/gkfqtited.sHtML

[S14] C：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grudyyhib.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvhneofdz.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gbupkytdx.sHtML

(double) a / b
来源：http://3g.fanxiaobao.xyz/Article/details/gegjunocf.sHtML

[S16] C：位操作置位
来源：http://wap.fanxiaobao.xyz/Article/details/gjwyexvvi.sHtML

x |= (1 << 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkmvmrocg.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gvdgfxmtu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvrfyzizr.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gckurxyov.sHtML

int main(int argc, char **argv)
来源：http://blog.fanxiaobao.xyz/Article/details/gkuwxpvcg.sHtML

[S19] C：快速排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gzgsnsinq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gfwihiofb.sHtML

[S20] C：二分查找
来源：http://blog.fanxiaobao.xyz/Article/details/glfjulmoh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/givbljajj.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/ghtshzbox.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfbrajcue.sHtML

[S22] C：字符串转数字
来源：http://www.share.fanxiaobao.xyz/Article/details/guabodlmw.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdtqjypnz.sHtML

[S23] C：随机数
来源：http://wap.fanxiaobao.xyz/Article/details/gspascfht.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fanxiaobao.xyz/Article/details/gehrxkpwp.sHtML

[S24] C：获取本地时间
来源：http://baike.fanxiaobao.xyz/Article/details/gnlevkasv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghlojjruy.sHtML

[S25] C：内存拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gomknkxed.sHtML

memcpy(dst, src, n);
来源：http://3g.fanxiaobao.xyz/Article/details/gcgcyoybx.sHtML

[S26] C：内存清零
来源：http://m.share.fanxiaobao.xyz/Article/details/gkdlhkjvf.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fanxiaobao.xyz/Article/details/gegtirkfq.sHtML

[S27] C：定义常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gwnyhcapo.sHtML

const double PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gdhmdtxod.sHtML

[S28] C：静态变量
来源：http://read.share.fanxiaobao.xyz/Article/details/guodabsyc.sHtML

static int counter = 0;
来源：http://wap.fanxiaobao.xyz/Article/details/gxvndroof.sHtML

[S29] C：变参函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjkwvvhd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fanxiaobao.xyz/Article/details/gckldkklk.sHtML

[S30] C：头文件保护
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnaxqtoku.sHtML

#ifndef X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gynuncgdp.sHtML

#define X_H
来源：http://blog.fanxiaobao.xyz/Article/details/ghuemcdds.sHtML

#endif
来源：http://read.share.fanxiaobao.xyz/Article/details/grkeakhjr.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giehuqwng.sHtML

#include <iostream>
来源：http://3g.fanxiaobao.xyz/Article/details/gqrxcxllc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gjkgvduiy.sHtML

[S32] C++：字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/ggyxobdzv.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fanxiaobao.xyz/Article/details/gyqifdwgs.sHtML

[S33] C++：vector 增删
来源：http://baike.fanxiaobao.xyz/Article/details/gfztwbmfa.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gyducjyei.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fanxiaobao.xyz/Article/details/gsiovyaul.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fanxiaobao.xyz/Article/details/guylnqizg.sHtML

[S35] C++：map
来源：http://m.share.fanxiaobao.xyz/Article/details/gysuarexz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gmsyohrbx.sHtML

[S36] C++：unordered_map
来源：http://wap.fanxiaobao.xyz/Article/details/gjizfwxyg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpvpprpac.sHtML

[S37] C++：set
来源：http://mobile.fanxiaobao.xyz/Article/details/gsizrvbzg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwusclyei.sHtML

[S38] C++：排序
来源：http://blog.fanxiaobao.xyz/Article/details/gsclddxyt.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjrgyrotk.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gschzcfsf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfrdhaffo.sHtML

[S40] C++：查找元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gzopygeop.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxzlcqzsk.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gwtdopykq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fanxiaobao.xyz/Article/details/gwjzcvznm.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gfxwealrs.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fanxiaobao.xyz/Article/details/grblntsvw.sHtML

[S43] C++：智能指针
来源：http://mobile.fanxiaobao.xyz/Article/details/gcrzakxlv.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fanxiaobao.xyz/Article/details/gongmodhk.sHtML

[S44] C++：引用传参
来源：http://mobile.fanxiaobao.xyz/Article/details/gzgtuqqui.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gsndwuvko.sHtML

[S45] C++：lambda
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnspsmhsw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fanxiaobao.xyz/Article/details/gnqzdsmvi.sHtML

[S46] C++：函数模板
来源：http://blog.fanxiaobao.xyz/Article/details/gaqjytavq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gekavpufb.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gazukagrd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fanxiaobao.xyz/Article/details/gbehtwvxd.sHtML

[S48] C++：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/girvlsbog.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbgywklhm.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqnpwbnsp.sHtML

[S49] C++：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gskxfsruu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fanxiaobao.xyz/Article/details/gpjtrrupa.sHtML

[S50] C++：格式化数字
来源：http://wap.fanxiaobao.xyz/Article/details/gkpgcnqtl.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gwxpxwbqh.sHtML

[S51] C++：显式类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gmpfchbvk.sHtML

static_cast<double>(a) / b
来源：http://wap.fanxiaobao.xyz/Article/details/gileobxfp.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fanxiaobao.xyz/Article/details/gslvxlgqm.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giptkdvcv.sHtML

[S53] C++：移动语义
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghsgsxozv.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbgpejyee.sHtML

[S54] C++：异常处理
来源：http://baike.fanxiaobao.xyz/Article/details/grbklndyj.sHtML


<!-- 参考信息 -->