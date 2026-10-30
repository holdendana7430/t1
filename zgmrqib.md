代发 wailian999

[Q86] 读取 JSON 字段
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwtnkxhy.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.fanxiaobao.xyz/Article/details/gqowpalsw.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gmbynlzpr.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtvztdreg.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fanxiaobao.xyz/Article/details/gkwnfbtig.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fanxiaobao.xyz/Article/details/gqixhjcgg.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gpklzvczj.sHtML

[Q89] 判断表是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gebnasnms.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fanxiaobao.xyz/Article/details/gskumipzt.sHtML

[Q90] 生成序号列
来源：http://blog.fanxiaobao.xyz/Article/details/gmmtlwjsr.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkpflbynz.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnlgehdac.sHtML

R. Bash 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjutdsai.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gnntsczzl.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fanxiaobao.xyz/Article/details/gnxxdzkuc.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdapuvzfa.sHtML

set -euo pipefail
来源：http://blog.fanxiaobao.xyz/Article/details/gpkyqogpo.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxowjysyp.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdtjhzduu.sHtML

[R03] 只读变量
来源：http://wap.fanxiaobao.xyz/Article/details/gcdcyzdch.sHtML

readonly PI=3.14
来源：http://3g.fanxiaobao.xyz/Article/details/gdndawqhq.sHtML

[R04] 位置参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxgbmlxag.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsfmkjnnw.sHtML

[R05] 参数默认值
来源：http://baike.fanxiaobao.xyz/Article/details/gpimvcfiq.sHtML

name="${1:-default}"
来源：http://wap.fanxiaobao.xyz/Article/details/gfdbpcqwa.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcrnertkd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gsgezzelw.sHtML

[R07] if 判断文件
来源：http://m.share.fanxiaobao.xyz/Article/details/giuyvldrz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gwgzznibc.sHtML

[R08] 数值比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gatxhwjqz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwwprlck.sHtML

[R09] 字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gtdfjmycl.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geyjmgolv.sHtML

[R10] 正则匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gnpulusbk.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnclliyga.sHtML

[R11] case 多分支
来源：http://3g.fanxiaobao.xyz/Article/details/gbylaupvc.sHtML

case "$1" in
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxlrsywow.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsfttguxo.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxbnwmazj.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcxmecxrl.sHtML

esac
来源：http://www.share.fanxiaobao.xyz/Article/details/glcrzwdwq.sHtML

[R12] for 遍历文件
来源：http://m.share.fanxiaobao.xyz/Article/details/grxobbnmj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glvpnkngp.sHtML

[R13] for 计数循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gergjnanf.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gweyheuzx.sHtML

[R14] C 风格 for
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxbamgeo.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gohwnalkb.sHtML

[R15] while 逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gldnwyrct.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gvkimzeqx.sHtML

[R16] until 等待条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbombqzvc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/goosxbxyy.sHtML

[R17] 数组定义与取值
来源：http://www.share.fanxiaobao.xyz/Article/details/gucqwpdut.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gyiblmoje.sHtML

[R18] 遍历数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gnexukdfc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkhjhpijn.sHtML

[R19] 数组长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gbcdnwcgj.sHtML

echo "${#arr[@]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gwylttojw.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gorpxpvbj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/geinyyzxt.sHtML

[R21] 字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gcpdkdpdj.sHtML

echo "${#s}"
来源：http://baike.fanxiaobao.xyz/Article/details/ggiqbmkao.sHtML

[R22] 截取子串
来源：http://baike.fanxiaobao.xyz/Article/details/govoggism.sHtML

echo "${s:0:5}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdgylxpdu.sHtML

[R23] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gsdzhejca.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fanxiaobao.xyz/Article/details/gfauyjziq.sHtML

[R24] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gnwoqzrba.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fanxiaobao.xyz/Article/details/glqnqwcjp.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvactkfhl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/galfvfyoy.sHtML

[R26] 命令替换
来源：http://wap.fanxiaobao.xyz/Article/details/grosilsnu.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fanxiaobao.xyz/Article/details/gjuuzbsyg.sHtML

[R27] 算术展开
来源：http://wap.fanxiaobao.xyz/Article/details/gmpubndti.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvajhkkrc.sHtML

[R28] 浮点运算
来源：http://www.share.fanxiaobao.xyz/Article/details/geofyccbl.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fanxiaobao.xyz/Article/details/gqluhkvjh.sHtML

[R29] 定义函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gkxaebapi.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gfxlvbjwu.sHtML

[R30] 函数返回状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gkwnrtofi.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkfrtslmg.sHtML

[R31] 局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gscxdttxz.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fanxiaobao.xyz/Article/details/glvrqqlrq.sHtML

[R32] 参数个数校验
来源：http://www.share.fanxiaobao.xyz/Article/details/gmbpeeatu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gosqlrkzg.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gmzmfcrpa.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fanxiaobao.xyz/Article/details/gihwjprgk.sHtML

[R34] 退出时清理
来源：http://read.share.fanxiaobao.xyz/Article/details/gsevlkndl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdwvvmqw.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehsellka.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fanxiaobao.xyz/Article/details/gohegmtjk.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/galnnixqn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fanxiaobao.xyz/Article/details/gtttkysjg.sHtML

[R37] 把输出赋给变量
来源：http://wap.fanxiaobao.xyz/Article/details/gxvxstxfp.sHtML

files=$(ls -1)
来源：http://blog.fanxiaobao.xyz/Article/details/gyqzegora.sHtML

[R38] 管道串联
来源：http://wap.fanxiaobao.xyz/Article/details/gcsdsijzf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gwuzsrhpo.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fanxiaobao.xyz/Article/details/ghrimvfqu.sHtML

cmd > out.log 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/grrhvmhyh.sHtML

[R40] 追加写日志
来源：http://baike.fanxiaobao.xyz/Article/details/glxkfircy.sHtML

echo "log" >> out.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gdqltrjcb.sHtML

[R41] 丢弃输出
来源：http://baike.fanxiaobao.xyz/Article/details/gpttezdki.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/galnsnwcb.sHtML

[R42] 输入重定向
来源：http://www.share.fanxiaobao.xyz/Article/details/gbrutewnc.sHtML

wc -l < a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gphwuvxdv.sHtML

[R43] 按名字查找文件
来源：http://blog.fanxiaobao.xyz/Article/details/gehcursll.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gewkbtvho.sHtML

[R44] 按修改时间查找
来源：http://3g.fanxiaobao.xyz/Article/details/gpzzmyidd.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnogzxmet.sHtML

[R45] 批量删除
来源：http://wap.fanxiaobao.xyz/Article/details/gmunefxmp.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fanxiaobao.xyz/Article/details/gplqwqkcu.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fanxiaobao.xyz/Article/details/gjukxxkvi.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyeghbtdx.sHtML

[R47] sed 单行替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gywvojhtt.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gufkuioha.sHtML

[R48] awk 取指定列
来源：http://mobile.fanxiaobao.xyz/Article/details/geercubcp.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gngkzpmew.sHtML

[R49] awk 带条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gphviboit.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fanxiaobao.xyz/Article/details/gjznycenc.sHtML

[R50] awk 求和
来源：http://baike.fanxiaobao.xyz/Article/details/gdjzsbhvp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/giztdlxts.sHtML

[R51] 排序去重取前几
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwiolquh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgneycjk.sHtML

[R52] 统计行数
来源：http://read.share.fanxiaobao.xyz/Article/details/gkgkgqmgb.sHtML

wc -l a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzwuewua.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fanxiaobao.xyz/Article/details/ghtfhcpte.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fanxiaobao.xyz/Article/details/gjwnrzvoq.sHtML

[R54] 比较两个文件
来源：http://wap.fanxiaobao.xyz/Article/details/gyrpqwrbf.sHtML

diff a.txt b.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmircdxr.sHtML

[R55] 压缩与解压
来源：http://wap.fanxiaobao.xyz/Article/details/gwowkxdge.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fanxiaobao.xyz/Article/details/ghvioedor.sHtML

[R56] 远程拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/ghtjzpyme.sHtML

scp file user@host:/path/
来源：http://baike.fanxiaobao.xyz/Article/details/gwjtziike.sHtML

[R57] 远程执行命令
来源：http://www.blog.fanxiaobao.xyz/Article/details/gysdyfans.sHtML

ssh user@host 'uptime'
来源：http://mobile.fanxiaobao.xyz/Article/details/gcdajtwor.sHtML

[R58] 下载文件
来源：http://wap.fanxiaobao.xyz/Article/details/gdcjplkwz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fanxiaobao.xyz/Article/details/gokkulgwk.sHtML

[R59] 发 POST JSON
来源：http://3g.fanxiaobao.xyz/Article/details/gzacfgdgc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/gfmvbwdie.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gptncvwrg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gobwwzmwh.sHtML

[R61] 磁盘占用
来源：http://3g.fanxiaobao.xyz/Article/details/govbktpso.sHtML

df -h;  du -sh *
来源：http://blog.fanxiaobao.xyz/Article/details/gpgzmmhkn.sHtML

[R62] 找最占空间的文件
来源：http://wap.fanxiaobao.xyz/Article/details/ggqrpvvnv.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fanxiaobao.xyz/Article/details/gpceutrtk.sHtML

[R63] 内存与进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmmfsyquk.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzfweubzh.sHtML

[R64] 结束进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gydyhbhoj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbuqnqcsp.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggcscdmys.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fanxiaobao.xyz/Article/details/gnqxdckna.sHtML

[R66] 定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/gpokszdny.sHtML

crontab -e;  crontab -l
来源：http://3g.fanxiaobao.xyz/Article/details/gorqudmec.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fanxiaobao.xyz/Article/details/gxzcaxjwc.sHtML

openssl rand -hex 16
来源：http://wap.fanxiaobao.xyz/Article/details/ggestnvmh.sHtML

[R68] 计算文件校验值
来源：http://wap.fanxiaobao.xyz/Article/details/gwxynpfpn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/ghgrgoxjj.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqvyxomh.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fanxiaobao.xyz/Article/details/giqvxvkiu.sHtML

[R70] 时间戳与互转
来源：http://mobile.fanxiaobao.xyz/Article/details/gmmaxvldo.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fanxiaobao.xyz/Article/details/gmfitustn.sHtML

[R71] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcnmddjxx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fanxiaobao.xyz/Article/details/gonbgxxym.sHtML

[R72] 等待端口就绪
来源：http://mobile.fanxiaobao.xyz/Article/details/gkbxdelva.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guytxsnzl.sHtML

[R73] 分割大日志
来源：http://3g.fanxiaobao.xyz/Article/details/gqncsurhf.sHtML

split -l 1000 big.log part_
来源：http://m.share.fanxiaobao.xyz/Article/details/gbxavifmj.sHtML

[R74] 批量重命名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnjzxfhwx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwmcivcyk.sHtML

[R75] 导出环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghpcgzmwr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/ggdfupfbp.sHtML

[R76] 使用临时文件
来源：http://baike.fanxiaobao.xyz/Article/details/gkosxlqjk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gycbecwwd.sHtML

[R77] 读取用户输入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzlgewrip.sHtML

read -rp "请输入: " ans
来源：http://m.share.fanxiaobao.xyz/Article/details/gipprvyqt.sHtML

[R78] 交互式菜单
来源：http://mobile.fanxiaobao.xyz/Article/details/gpjveajff.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fanxiaobao.xyz/Article/details/getvreliq.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwhaynsg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fanxiaobao.xyz/Article/details/ggutxlztj.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fanxiaobao.xyz/Article/details/geyscomak.sHtML

time ./run.sh
来源：http://www.share.fanxiaobao.xyz/Article/details/gspuvymcl.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/ghoprqwoc.sHtML

S. C / C++ 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gzewyowpq.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyoknlzgw.sHtML

[S01] C：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/ggilmizvb.sHtML

#include <stdio.h>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyorfzfgt.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fanxiaobao.xyz/Article/details/gsfsykyyl.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/gtsprpris.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggmjibolf.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gytnfelxl.sHtML

int x; scanf("%d", &x);
来源：http://3g.fanxiaobao.xyz/Article/details/gljuwskqj.sHtML

[S04] C：字符串复制
来源：http://mobile.fanxiaobao.xyz/Article/details/glqgmgfxg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fanxiaobao.xyz/Article/details/ghdphhotp.sHtML

[S05] C：字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gcgrzoiif.sHtML

strlen(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaglcdafv.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfahyjwsn.sHtML

strcmp(a, b) == 0
来源：http://mobile.fanxiaobao.xyz/Article/details/guyssoslp.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/gbhxgxcay.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fanxiaobao.xyz/Article/details/gyiqypxae.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjlnommy.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzndhztfy.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fanxiaobao.xyz/Article/details/gmhhyloee.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fanxiaobao.xyz/Article/details/gjoysxjqw.sHtML

[S10] C：指针与解引用
来源：http://www.share.fanxiaobao.xyz/Article/details/gayxexsbn.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fanxiaobao.xyz/Article/details/gyqxrvnna.sHtML

[S11] C：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gdkbiqrcl.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fanxiaobao.xyz/Article/details/gmjuyfreq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzsjhswi.sHtML

fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gyyidmizh.sHtML

[S12] C：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gailuqtbk.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gefgufxjt.sHtML

[S13] C：宏定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjlszfut.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fanxiaobao.xyz/Article/details/gkfexwzxq.sHtML

[S14] C：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gpeklzzbq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fanxiaobao.xyz/Article/details/gdmkppvix.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gtuwzmdsp.sHtML

(double) a / b
来源：http://blog.fanxiaobao.xyz/Article/details/glutrbcit.sHtML

[S16] C：位操作置位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpnbxfaca.sHtML

x |= (1 << 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnwqenjcc.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gkhrijqwd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fanxiaobao.xyz/Article/details/grwinnqgw.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzrsfhtam.sHtML

int main(int argc, char **argv)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvjrjygyh.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/gygnxohcr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/glpcmddnr.sHtML

[S20] C：二分查找
来源：http://wap.fanxiaobao.xyz/Article/details/gtbuiycvl.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwcnwxhrr.sHtML

[S21] C：字符类别判断
来源：http://blog.fanxiaobao.xyz/Article/details/ghqfpnsrj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnzlmiyrs.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggspbefhy.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fanxiaobao.xyz/Article/details/gcbaiixue.sHtML

[S23] C：随机数
来源：http://wap.fanxiaobao.xyz/Article/details/ghiokvbcc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjyhbdpzt.sHtML

[S24] C：获取本地时间
来源：http://read.share.fanxiaobao.xyz/Article/details/ghzrhwyda.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fanxiaobao.xyz/Article/details/gsatqurza.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gscidfxmy.sHtML

memcpy(dst, src, n);
来源：http://wap.fanxiaobao.xyz/Article/details/giammjtfr.sHtML

[S26] C：内存清零
来源：http://mobile.fanxiaobao.xyz/Article/details/gubjcasnd.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbfdhjlx.sHtML

[S27] C：定义常量
来源：http://baike.fanxiaobao.xyz/Article/details/gwnguyimh.sHtML

const double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/guflwozvb.sHtML

[S28] C：静态变量
来源：http://blog.fanxiaobao.xyz/Article/details/gsqeaivkw.sHtML

static int counter = 0;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghpyvhutj.sHtML

[S29] C：变参函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsztixdst.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkyzrugmg.sHtML

[S30] C：头文件保护
来源：http://blog.fanxiaobao.xyz/Article/details/grlognuil.sHtML

#ifndef X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gndicrtig.sHtML

#define X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gkmtnmddr.sHtML

#endif
来源：http://blog.fanxiaobao.xyz/Article/details/gyqtfqyua.sHtML

[S31] C++：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gnftaxcvx.sHtML

#include <iostream>
来源：http://baike.fanxiaobao.xyz/Article/details/gsyorbmrw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaporxckr.sHtML

[S32] C++：字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gibdydzun.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fanxiaobao.xyz/Article/details/gxvsdbufc.sHtML

[S33] C++：vector 增删
来源：http://read.share.fanxiaobao.xyz/Article/details/grvriagzs.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gcjvfakjr.sHtML

[S34] C++：遍历 vector
来源：http://blog.fanxiaobao.xyz/Article/details/griapqnle.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsywmrdje.sHtML

[S35] C++：map
来源：http://wap.fanxiaobao.xyz/Article/details/gshvwntyz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdzhekdus.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfkkwycgp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjrbdxdpb.sHtML

[S37] C++：set
来源：http://baike.fanxiaobao.xyz/Article/details/gojwugtfy.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gtmquvlqn.sHtML

[S38] C++：排序
来源：http://baike.fanxiaobao.xyz/Article/details/gxlsgpkvk.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/ggikquldt.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fanxiaobao.xyz/Article/details/gsfdsdzbm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fanxiaobao.xyz/Article/details/gmqjxefpd.sHtML

[S40] C++：查找元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzdjdutxh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fanxiaobao.xyz/Article/details/glqiwuvii.sHtML

[S41] C++：类与构造函数
来源：http://wap.fanxiaobao.xyz/Article/details/gscpfqpuj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gkejxobqd.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gntacykim.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/gqvbiutbu.sHtML

[S43] C++：智能指针
来源：http://blog.fanxiaobao.xyz/Article/details/guslsoxnm.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfynxcmuc.sHtML

[S44] C++：引用传参
来源：http://mobile.fanxiaobao.xyz/Article/details/gmbumadft.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gdgadtepd.sHtML

[S45] C++：lambda
来源：http://blog.fanxiaobao.xyz/Article/details/guhrzqllq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqavaeet.sHtML

[S46] C++：函数模板
来源：http://blog.fanxiaobao.xyz/Article/details/ggaxsysbz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gaeonvztk.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gwyrfxbdh.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fanxiaobao.xyz/Article/details/gjrzwghhj.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gcnowtfhc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fanxiaobao.xyz/Article/details/gspwjkcca.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/grjtfwabd.sHtML

[S49] C++：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gxdbumchp.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/glxrrubhq.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfnbgelza.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/giepztnea.sHtML

[S51] C++：显式类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gitooytyg.sHtML

static_cast<double>(a) / b
来源：http://wap.fanxiaobao.xyz/Article/details/gopprrizp.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fanxiaobao.xyz/Article/details/gwlqbkawh.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gyvivbozm.sHtML

[S53] C++：移动语义
来源：http://3g.fanxiaobao.xyz/Article/details/gxcvdpvqi.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fanxiaobao.xyz/Article/details/gbeiqvqtt.sHtML

[S54] C++：异常处理
来源：http://wap.fanxiaobao.xyz/Article/details/giyjwfkwq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmhgnxgt.sHtML

[S55] C++：结构化绑定
来源：http://wap.fanxiaobao.xyz/Article/details/gkapwjsak.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gpgvqiaqy.sHtML

[S56] C++：optional
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glagysrse.sHtML


<!-- 参考信息 -->