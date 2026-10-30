代发 wailian999

[Q86] 读取 JSON 字段
来源：http://blog.fehbvm.com/Article/details/gnexjknro.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.zdbjq.cn/Article/details/gehvkowsp.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.zdbjq.cn/Article/details/gwkkwlltc.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fehbvm.com/Article/details/goovsqiti.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.hesvh.cn/Article/details/gewnrgfvk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.hesvh.cn/Article/details/gzopgogko.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.hesvh.cn/Article/details/gnhqxtvpu.sHtML

[Q89] 判断表是否存在
来源：http://wap.fehbvm.com/Article/details/gjntwmqhy.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/gmxkdbvnl.sHtML

[Q90] 生成序号列
来源：http://www.blog.zdbjq.cn/Article/details/gtgppwfin.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.zdbjq.cn/Article/details/gjsimcyjz.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gxuhavuxc.sHtML

R. Bash 专题
来源：http://wap.zdbjq.cn/Article/details/gotvxrmpg.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gyzekoskh.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fehbvm.com/Article/details/gjptpqfdd.sHtML

#!/usr/bin/env bash
来源：http://blog.hesvh.cn/Article/details/gbmdwfsbl.sHtML

set -euo pipefail
来源：http://blog.zdbjq.cn/Article/details/gksljbmyv.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.hesvh.cn/Article/details/gcejhngbi.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.hesvh.cn/Article/details/ghupanxqx.sHtML

[R03] 只读变量
来源：http://wap.zdbjq.cn/Article/details/gyvtzahaa.sHtML

readonly PI=3.14
来源：http://baike.zdbjq.cn/Article/details/gbjrmjiho.sHtML

[R04] 位置参数
来源：http://www.m.share.fehbvm.com/Article/details/gftrmldzf.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.zdbjq.cn/Article/details/gbedxzopa.sHtML

[R05] 参数默认值
来源：http://m.share.zdbjq.cn/Article/details/gabjqbwsh.sHtML

name="${1:-default}"
来源：http://m.share.fehbvm.com/Article/details/gepsdcrje.sHtML

[R06] 判断命令是否存在
来源：http://3g.fehbvm.com/Article/details/gkiphtuok.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/geyonieuz.sHtML

[R07] if 判断文件
来源：http://www.share.hesvh.cn/Article/details/gronduzci.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gkpldbdeb.sHtML

[R08] 数值比较
来源：http://m.share.hesvh.cn/Article/details/gmzedkyrb.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gijewzrma.sHtML

[R09] 字符串比较
来源：http://m.share.hesvh.cn/Article/details/gzdvbuesp.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.zdbjq.cn/Article/details/gtxdrpaac.sHtML

[R10] 正则匹配
来源：http://www.blog.zdbjq.cn/Article/details/glvnwdncy.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fehbvm.com/Article/details/gwpzkcdwa.sHtML

[R11] case 多分支
来源：http://www.share.fehbvm.com/Article/details/grvpjyzxx.sHtML

case "$1" in
来源：http://www.blog.hesvh.cn/Article/details/gmvfnomdg.sHtML

start) echo "启动" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gsvmafqhm.sHtML

stop)  echo "停止" ;;
来源：http://m.share.zdbjq.cn/Article/details/gupfhnyjg.sHtML

*)     echo "未知命令" ;;
来源：http://blog.zdbjq.cn/Article/details/gbokinahi.sHtML

esac
来源：http://3g.fehbvm.com/Article/details/gepbwzvmc.sHtML

[R12] for 遍历文件
来源：http://wap.hesvh.cn/Article/details/gpzzyywmd.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.zdbjq.cn/Article/details/gsdxbmzkq.sHtML

[R13] for 计数循环
来源：http://m.share.hesvh.cn/Article/details/grynktbck.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gfonapryl.sHtML

[R14] C 风格 for
来源：http://m.share.hesvh.cn/Article/details/gylttkzuj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/gjfbnfjgy.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gvhmlfeeg.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.zdbjq.cn/Article/details/gsqvxiqrb.sHtML

[R16] until 等待条件
来源：http://wap.zdbjq.cn/Article/details/ghozpoycc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/gteimnimy.sHtML

[R17] 数组定义与取值
来源：http://mobile.hesvh.cn/Article/details/gcwrrazzl.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.hesvh.cn/Article/details/gculcmhtv.sHtML

[R18] 遍历数组
来源：http://wap.zdbjq.cn/Article/details/gfawkpord.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fehbvm.com/Article/details/gdisrnndv.sHtML

[R19] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/gjrebvpki.sHtML

echo "${#arr[@]}"
来源：http://read.share.zdbjq.cn/Article/details/grflqhrdr.sHtML

[R20] 关联数组（字典）
来源：http://baike.hesvh.cn/Article/details/glnxaajda.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.zdbjq.cn/Article/details/gmseulmvf.sHtML

[R21] 字符串长度
来源：http://wap.zdbjq.cn/Article/details/ggnwiqcrd.sHtML

echo "${#s}"
来源：http://mobile.zdbjq.cn/Article/details/grsinivaq.sHtML

[R22] 截取子串
来源：http://mobile.hesvh.cn/Article/details/gbgizdoev.sHtML

echo "${s:0:5}"
来源：http://www.share.zdbjq.cn/Article/details/ggdqantiu.sHtML

[R23] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/gjbxcemzm.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fehbvm.com/Article/details/gpdaotcft.sHtML

[R24] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gwsfgaesz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fehbvm.com/Article/details/gwbrldzoq.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.zdbjq.cn/Article/details/gvifuefax.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fehbvm.com/Article/details/gzuisixmu.sHtML

[R26] 命令替换
来源：http://baike.hesvh.cn/Article/details/gzyfklwil.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.hesvh.cn/Article/details/gefceysqk.sHtML

[R27] 算术展开
来源：http://wap.fehbvm.com/Article/details/gzxgklxha.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.hesvh.cn/Article/details/gktzfkrxz.sHtML

[R28] 浮点运算
来源：http://blog.fehbvm.com/Article/details/gaqgmzwlo.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.zdbjq.cn/Article/details/gcfzohrnq.sHtML

[R29] 定义函数
来源：http://3g.zdbjq.cn/Article/details/gicooflix.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fehbvm.com/Article/details/gxlffskez.sHtML

[R30] 函数返回状态码
来源：http://read.share.fehbvm.com/Article/details/gohfmrleh.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.zdbjq.cn/Article/details/gdbfzxclc.sHtML

[R31] 局部变量
来源：http://wap.fehbvm.com/Article/details/gfhrmkmxp.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.hesvh.cn/Article/details/gswnkjcwx.sHtML

[R32] 参数个数校验
来源：http://baike.zdbjq.cn/Article/details/gtvbfyyru.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gqrjxgink.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fehbvm.com/Article/details/gjguafujl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.zdbjq.cn/Article/details/grrxuylra.sHtML

[R34] 退出时清理
来源：http://3g.fehbvm.com/Article/details/gkhputacb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gggvcemhc.sHtML

[R35] 后台执行并等待
来源：http://baike.zdbjq.cn/Article/details/gmokvztck.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fehbvm.com/Article/details/gndvocrku.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fehbvm.com/Article/details/gxlrohfli.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.zdbjq.cn/Article/details/gxdxzrngi.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fehbvm.com/Article/details/gcjjoekls.sHtML

files=$(ls -1)
来源：http://wap.hesvh.cn/Article/details/gfcqexvab.sHtML

[R38] 管道串联
来源：http://mobile.zdbjq.cn/Article/details/giuabpcpj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fehbvm.com/Article/details/gidwcvndg.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fehbvm.com/Article/details/gdffgmczx.sHtML

cmd > out.log 2>&1
来源：http://3g.hesvh.cn/Article/details/gslyfynew.sHtML

[R40] 追加写日志
来源：http://www.m.share.zdbjq.cn/Article/details/gqjpcvqhx.sHtML

echo "log" >> out.log
来源：http://wap.fehbvm.com/Article/details/gtcvcdfvl.sHtML

[R41] 丢弃输出
来源：http://baike.zdbjq.cn/Article/details/gslalkkdc.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fehbvm.com/Article/details/gddhzvkpe.sHtML

[R42] 输入重定向
来源：http://baike.hesvh.cn/Article/details/ghrcbkikp.sHtML

wc -l < a.txt
来源：http://blog.hesvh.cn/Article/details/gjtqdxoqz.sHtML

[R43] 按名字查找文件
来源：http://mobile.hesvh.cn/Article/details/gpofhjbxc.sHtML

find . -name "*.log" -type f
来源：http://3g.fehbvm.com/Article/details/gglrkmwnw.sHtML

[R44] 按修改时间查找
来源：http://read.share.fehbvm.com/Article/details/gpelzzubq.sHtML

find . -mtime -7 -type f
来源：http://www.blog.hesvh.cn/Article/details/gbhxlnbpk.sHtML

[R45] 批量删除
来源：http://www.blog.zdbjq.cn/Article/details/gfzkciqqo.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fehbvm.com/Article/details/gsificwec.sHtML

[R46] 递归替换文件内容
来源：http://3g.zdbjq.cn/Article/details/glzukjedz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.hesvh.cn/Article/details/gycsczqkq.sHtML

[R47] sed 单行替换
来源：http://blog.hesvh.cn/Article/details/gqwmbpzzp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gasakilxt.sHtML

[R48] awk 取指定列
来源：http://mobile.fehbvm.com/Article/details/gwbtbjatx.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fehbvm.com/Article/details/gpihoqzyn.sHtML

[R49] awk 带条件
来源：http://m.share.fehbvm.com/Article/details/gfjltidca.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.zdbjq.cn/Article/details/gtzkvfgkw.sHtML

[R50] awk 求和
来源：http://blog.fehbvm.com/Article/details/gtnletoeb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gvocihosr.sHtML

[R51] 排序去重取前几
来源：http://read.share.hesvh.cn/Article/details/gzipmyrfg.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fehbvm.com/Article/details/gqzbijoam.sHtML

[R52] 统计行数
来源：http://wap.zdbjq.cn/Article/details/gwibaqkwl.sHtML

wc -l a.txt
来源：http://mobile.zdbjq.cn/Article/details/gaophdvlx.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fehbvm.com/Article/details/gdtgefupr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fehbvm.com/Article/details/grvtrokqe.sHtML

[R54] 比较两个文件
来源：http://www.share.fehbvm.com/Article/details/graktymcb.sHtML

diff a.txt b.txt
来源：http://www.m.share.fehbvm.com/Article/details/ggacpuxur.sHtML

[R55] 压缩与解压
来源：http://m.share.zdbjq.cn/Article/details/gdcbvaurp.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.zdbjq.cn/Article/details/glzhvywql.sHtML

[R56] 远程拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gosrbdfjn.sHtML

scp file user@host:/path/
来源：http://www.blog.hesvh.cn/Article/details/gfstalnnx.sHtML

[R57] 远程执行命令
来源：http://wap.zdbjq.cn/Article/details/gsuieactw.sHtML

ssh user@host 'uptime'
来源：http://read.share.fehbvm.com/Article/details/gswdjrkzj.sHtML

[R58] 下载文件
来源：http://blog.hesvh.cn/Article/details/gavjzitio.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.zdbjq.cn/Article/details/gstnmkbsc.sHtML

[R59] 发 POST JSON
来源：http://baike.fehbvm.com/Article/details/gdeyokydd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fehbvm.com/Article/details/gamgieaar.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.zdbjq.cn/Article/details/gbeeidfco.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.zdbjq.cn/Article/details/gwgxzumxb.sHtML

[R61] 磁盘占用
来源：http://wap.fehbvm.com/Article/details/gxfrfxsay.sHtML

df -h;  du -sh *
来源：http://www.m.share.zdbjq.cn/Article/details/gatrmkmxg.sHtML

[R62] 找最占空间的文件
来源：http://blog.fehbvm.com/Article/details/gaesxpbew.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.zdbjq.cn/Article/details/gstlvdztt.sHtML

[R63] 内存与进程
来源：http://www.blog.hesvh.cn/Article/details/gogpnrrae.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fehbvm.com/Article/details/givknlykh.sHtML

[R64] 结束进程
来源：http://read.share.hesvh.cn/Article/details/geciqwzuw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.hesvh.cn/Article/details/gbbljxceo.sHtML

[R65] 查看端口占用
来源：http://blog.hesvh.cn/Article/details/gthddkcve.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.zdbjq.cn/Article/details/gqgmaplbw.sHtML

[R66] 定时任务
来源：http://3g.hesvh.cn/Article/details/gpvfrzkca.sHtML

crontab -e;  crontab -l
来源：http://wap.zdbjq.cn/Article/details/giegjtumr.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.zdbjq.cn/Article/details/gamlmqhiw.sHtML

openssl rand -hex 16
来源：http://www.m.share.zdbjq.cn/Article/details/gxgljftcn.sHtML

[R68] 计算文件校验值
来源：http://read.share.fehbvm.com/Article/details/giazrpysl.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fehbvm.com/Article/details/guhwdxsfm.sHtML

[R69] 生成随机密码
来源：http://baike.hesvh.cn/Article/details/gsortqkpc.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.zdbjq.cn/Article/details/gpkwiddwc.sHtML

[R70] 时间戳与互转
来源：http://wap.zdbjq.cn/Article/details/glqeokxlw.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fehbvm.com/Article/details/gmjgexuga.sHtML

[R71] 日期格式化
来源：http://blog.fehbvm.com/Article/details/gsrqtfhek.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fehbvm.com/Article/details/gfilrjxfi.sHtML

[R72] 等待端口就绪
来源：http://blog.zdbjq.cn/Article/details/ghmqheqwd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/gmxjyaywm.sHtML

[R73] 分割大日志
来源：http://blog.hesvh.cn/Article/details/gxphxehxn.sHtML

split -l 1000 big.log part_
来源：http://blog.fehbvm.com/Article/details/ghzapzghg.sHtML

[R74] 批量重命名
来源：http://read.share.fehbvm.com/Article/details/gleycdedf.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fehbvm.com/Article/details/gyxihvlqh.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gznsnrfwn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.zdbjq.cn/Article/details/gwefggufh.sHtML

[R76] 使用临时文件
来源：http://3g.zdbjq.cn/Article/details/gbgfnxbpo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/gdahtjbso.sHtML

[R77] 读取用户输入
来源：http://www.blog.fehbvm.com/Article/details/gogcnfrya.sHtML

read -rp "请输入: " ans
来源：http://mobile.zdbjq.cn/Article/details/gplqbqemd.sHtML

[R78] 交互式菜单
来源：http://3g.hesvh.cn/Article/details/guwdyduja.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.hesvh.cn/Article/details/grqifcyyd.sHtML

[R79] 解析命令行选项
来源：http://www.share.zdbjq.cn/Article/details/gnjhvwodz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fehbvm.com/Article/details/gsxmrsshz.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.hesvh.cn/Article/details/ghznwliaf.sHtML

time ./run.sh
来源：http://www.m.share.fehbvm.com/Article/details/gfhuodbgl.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gwwzdckuf.sHtML

S. C / C++ 专题
来源：http://blog.zdbjq.cn/Article/details/gmcyniqxa.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gdnqlxrkq.sHtML

[S01] C：Hello World
来源：http://read.share.hesvh.cn/Article/details/gosggbhis.sHtML

#include <stdio.h>
来源：http://baike.fehbvm.com/Article/details/gxvaedjje.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fehbvm.com/Article/details/gbwvhpqsc.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fehbvm.com/Article/details/gptuuxwit.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fehbvm.com/Article/details/gpyjwptgx.sHtML

[S03] C：读入整数
来源：http://read.share.fehbvm.com/Article/details/gtkzbsjbu.sHtML

int x; scanf("%d", &x);
来源：http://m.share.zdbjq.cn/Article/details/gqwlkxjyj.sHtML

[S04] C：字符串复制
来源：http://www.m.share.hesvh.cn/Article/details/gylytygsv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fehbvm.com/Article/details/gpakojaii.sHtML

[S05] C：字符串长度
来源：http://wap.fehbvm.com/Article/details/gmuhccimz.sHtML

strlen(s)
来源：http://m.share.hesvh.cn/Article/details/gzjwojthh.sHtML

[S06] C：字符串比较
来源：http://baike.zdbjq.cn/Article/details/gawhoecxj.sHtML

strcmp(a, b) == 0
来源：http://blog.zdbjq.cn/Article/details/gcfudzsll.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fehbvm.com/Article/details/gfgwxibqz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.hesvh.cn/Article/details/gujdxazzm.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fehbvm.com/Article/details/gowgrlagn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fehbvm.com/Article/details/gkyfmxpgi.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.zdbjq.cn/Article/details/gpvtigtno.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.zdbjq.cn/Article/details/gnlwmmkwk.sHtML

[S10] C：指针与解引用
来源：http://www.share.fehbvm.com/Article/details/gombpfdak.sHtML

int *p = &a;  *p = 5;
来源：http://3g.zdbjq.cn/Article/details/gqhqqqril.sHtML

[S11] C：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gakhinoms.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.zdbjq.cn/Article/details/gwidmzqzf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fehbvm.com/Article/details/ggaiajtau.sHtML

fclose(f);
来源：http://wap.fehbvm.com/Article/details/gillltpyc.sHtML

[S12] C：写文件
来源：http://www.m.share.zdbjq.cn/Article/details/golgthtbu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/grghemmho.sHtML

[S13] C：宏定义
来源：http://baike.hesvh.cn/Article/details/gwyjwlggb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.hesvh.cn/Article/details/girfbomnd.sHtML

[S14] C：枚举
来源：http://www.blog.hesvh.cn/Article/details/gxzobymmd.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.hesvh.cn/Article/details/gzivecjuh.sHtML

[S15] C：类型转换
来源：http://www.m.share.fehbvm.com/Article/details/gwnppahaa.sHtML

(double) a / b
来源：http://blog.fehbvm.com/Article/details/glfwpawyv.sHtML

[S16] C：位操作置位
来源：http://baike.zdbjq.cn/Article/details/gkmwzzebf.sHtML

x |= (1 << 3);
来源：http://www.m.share.fehbvm.com/Article/details/ggajkruqn.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/ghcacabzi.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.hesvh.cn/Article/details/gtwvvtqoc.sHtML

[S18] C：命令行参数
来源：http://www.blog.hesvh.cn/Article/details/ghuqptzsi.sHtML

int main(int argc, char **argv)
来源：http://mobile.zdbjq.cn/Article/details/ggvfqwgin.sHtML

[S19] C：快速排序
来源：http://baike.fehbvm.com/Article/details/goyzrxoya.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/gbdvghzbl.sHtML

[S20] C：二分查找
来源：http://baike.zdbjq.cn/Article/details/gehuxigfl.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/gmizyoamu.sHtML

[S21] C：字符类别判断
来源：http://blog.hesvh.cn/Article/details/gkyvhsrmc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fehbvm.com/Article/details/gjcunclth.sHtML

[S22] C：字符串转数字
来源：http://www.share.hesvh.cn/Article/details/gokqchefx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.zdbjq.cn/Article/details/ghqgykpwz.sHtML

[S23] C：随机数
来源：http://baike.fehbvm.com/Article/details/glcfdyubd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.hesvh.cn/Article/details/gsblwpibx.sHtML

[S24] C：获取本地时间
来源：http://www.blog.zdbjq.cn/Article/details/gppcwokpq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fehbvm.com/Article/details/gqcansyqs.sHtML

[S25] C：内存拷贝
来源：http://m.share.fehbvm.com/Article/details/gblftyjxi.sHtML

memcpy(dst, src, n);
来源：http://wap.zdbjq.cn/Article/details/ggdbsnfrg.sHtML

[S26] C：内存清零
来源：http://www.blog.fehbvm.com/Article/details/gihxjlafj.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fehbvm.com/Article/details/gjincpptd.sHtML

[S27] C：定义常量
来源：http://www.share.fehbvm.com/Article/details/gpbbxdxnu.sHtML

const double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gzqvhfohw.sHtML

[S28] C：静态变量
来源：http://baike.hesvh.cn/Article/details/glmetxgea.sHtML

static int counter = 0;
来源：http://blog.fehbvm.com/Article/details/gpsnggnpv.sHtML

[S29] C：变参函数
来源：http://www.share.hesvh.cn/Article/details/gaarirrjd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.zdbjq.cn/Article/details/giwlwlyyc.sHtML

[S30] C：头文件保护
来源：http://wap.fehbvm.com/Article/details/govqdyxco.sHtML

#ifndef X_H
来源：http://www.share.hesvh.cn/Article/details/gpainihke.sHtML

#define X_H
来源：http://www.m.share.fehbvm.com/Article/details/geepbjcoo.sHtML

#endif
来源：http://www.share.zdbjq.cn/Article/details/gpmtbdvpd.sHtML

[S31] C++：Hello World
来源：http://mobile.fehbvm.com/Article/details/grkfwsuzi.sHtML

#include <iostream>
来源：http://mobile.fehbvm.com/Article/details/gybijgqhj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.zdbjq.cn/Article/details/gyhjhybxn.sHtML

[S32] C++：字符串
来源：http://www.share.hesvh.cn/Article/details/gijqmolqy.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fehbvm.com/Article/details/gkbeqbfmz.sHtML

[S33] C++：vector 增删
来源：http://m.share.zdbjq.cn/Article/details/gidoibdpz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.zdbjq.cn/Article/details/gzfqkhztr.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.zdbjq.cn/Article/details/gwluhdjnm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.hesvh.cn/Article/details/gtomsdviy.sHtML

[S35] C++：map
来源：http://read.share.zdbjq.cn/Article/details/gwqwmjaay.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/grbaugzol.sHtML

[S36] C++：unordered_map
来源：http://read.share.zdbjq.cn/Article/details/gyswskoyn.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gtwvdjefk.sHtML

[S37] C++：set
来源：http://www.m.share.fehbvm.com/Article/details/gydhnywvu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.hesvh.cn/Article/details/gyrptsfle.sHtML

[S38] C++：排序
来源：http://baike.hesvh.cn/Article/details/gsjaqgkru.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fehbvm.com/Article/details/geewrrrnf.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fehbvm.com/Article/details/glhdhegvq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.zdbjq.cn/Article/details/gbmstaklp.sHtML

[S40] C++：查找元素
来源：http://m.share.hesvh.cn/Article/details/glephtiab.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fehbvm.com/Article/details/gfqhidxuj.sHtML

[S41] C++：类与构造函数
来源：http://wap.hesvh.cn/Article/details/gwtwlosza.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.zdbjq.cn/Article/details/glskidasx.sHtML

[S42] C++：继承与虚函数
来源：http://baike.hesvh.cn/Article/details/gghlqryxf.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.hesvh.cn/Article/details/gbdvybbdv.sHtML

[S43] C++：智能指针
来源：http://www.blog.hesvh.cn/Article/details/gbdecflwy.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.hesvh.cn/Article/details/guqbpgkvt.sHtML

[S44] C++：引用传参
来源：http://www.blog.fehbvm.com/Article/details/gihpeysqy.sHtML

void inc(int &x) { ++x; }
来源：http://wap.hesvh.cn/Article/details/gdquwbmaj.sHtML

[S45] C++：lambda
来源：http://baike.zdbjq.cn/Article/details/giigcfqye.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fehbvm.com/Article/details/gklgergqm.sHtML

[S46] C++：函数模板
来源：http://3g.fehbvm.com/Article/details/ggaavumrp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fehbvm.com/Article/details/gxxbowxkt.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.zdbjq.cn/Article/details/gpawquxmf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.hesvh.cn/Article/details/gnhamyzyz.sHtML

[S48] C++：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gnywurupn.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.hesvh.cn/Article/details/gljsmmsmv.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.hesvh.cn/Article/details/gazwzyupr.sHtML

[S49] C++：写文件
来源：http://3g.zdbjq.cn/Article/details/gpfvcanch.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fehbvm.com/Article/details/gbwdxjhnt.sHtML

[S50] C++：格式化数字
来源：http://baike.zdbjq.cn/Article/details/gtwxakonp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fehbvm.com/Article/details/guhgytjwm.sHtML

[S51] C++：显式类型转换
来源：http://3g.zdbjq.cn/Article/details/gktzwvzlc.sHtML

static_cast<double>(a) / b
来源：http://mobile.hesvh.cn/Article/details/gzzjpzcuk.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.hesvh.cn/Article/details/gpdeyppxc.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.zdbjq.cn/Article/details/gajymlzag.sHtML

[S53] C++：移动语义
来源：http://www.share.hesvh.cn/Article/details/gtuoauviv.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.hesvh.cn/Article/details/grhdoestn.sHtML

[S54] C++：异常处理
来源：http://read.share.fehbvm.com/Article/details/gxtoulzzo.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.hesvh.cn/Article/details/gfgjtjhef.sHtML

[S55] C++：结构化绑定
来源：http://blog.zdbjq.cn/Article/details/gibojatng.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fehbvm.com/Article/details/ggbeclkun.sHtML

[S56] C++：optional
来源：http://blog.zdbjq.cn/Article/details/gwqqymphe.sHtML


<!-- 参考信息 -->