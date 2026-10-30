代发 wailian999

set -euo pipefail
来源：http://read.share.fanxiaobao.xyz/Article/details/gspljoloe.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fanxiaobao.xyz/Article/details/gugbtuufo.sHtML

name="Tom"; echo "$name"
来源：http://wap.fanxiaobao.xyz/Article/details/gggzwtmgr.sHtML

[R03] 只读变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gpqszpebe.sHtML

readonly PI=3.14
来源：http://read.share.fanxiaobao.xyz/Article/details/giwndsuag.sHtML

[R04] 位置参数
来源：http://3g.fanxiaobao.xyz/Article/details/goprcpwux.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fanxiaobao.xyz/Article/details/gswuwuapg.sHtML

[R05] 参数默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/ggwacjqxn.sHtML

name="${1:-default}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gdofwbvfm.sHtML

[R06] 判断命令是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gmiylzxcp.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gsqowddff.sHtML

[R07] if 判断文件
来源：http://blog.fanxiaobao.xyz/Article/details/gqeprwlrq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gttpoxzro.sHtML

[R08] 数值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gifuajjhz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gqjyrrcgf.sHtML

[R09] 字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gffodilrg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gofxqdjok.sHtML

[R10] 正则匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gaajjonex.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gpybagfku.sHtML

[R11] case 多分支
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtcnydrwh.sHtML

case "$1" in
来源：http://3g.fanxiaobao.xyz/Article/details/gqmfhftna.sHtML

start) echo "启动" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gpghllimd.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmolhzmzy.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gxoracyjp.sHtML

esac
来源：http://mobile.fanxiaobao.xyz/Article/details/gyrhkikbx.sHtML

[R12] for 遍历文件
来源：http://blog.fanxiaobao.xyz/Article/details/gcjhujrxu.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/geqceouiz.sHtML

[R13] for 计数循环
来源：http://wap.fanxiaobao.xyz/Article/details/gaaecgwcp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/glzowmxbe.sHtML

[R14] C 风格 for
来源：http://baike.fanxiaobao.xyz/Article/details/gjmkkwork.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gzagqqvuv.sHtML

[R15] while 逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gkttpgnly.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gbovmmcgy.sHtML

[R16] until 等待条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gsoakexhz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqrtftpyw.sHtML

[R17] 数组定义与取值
来源：http://wap.fanxiaobao.xyz/Article/details/gqdjuakil.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gmievijot.sHtML

[R18] 遍历数组
来源：http://blog.fanxiaobao.xyz/Article/details/gcgpgmgsw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gymqjlfay.sHtML

[R19] 数组长度
来源：http://3g.fanxiaobao.xyz/Article/details/gbxxwecza.sHtML

echo "${#arr[@]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gsdgmvxzw.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fanxiaobao.xyz/Article/details/gxhffvatk.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gqoteqaol.sHtML

[R21] 字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjovdvth.sHtML

echo "${#s}"
来源：http://wap.fanxiaobao.xyz/Article/details/gtlbthhws.sHtML

[R22] 截取子串
来源：http://www.share.fanxiaobao.xyz/Article/details/gwefdrihi.sHtML

echo "${s:0:5}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gtvczmhsf.sHtML

[R23] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/ggxmlikdg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gojafulav.sHtML

[R24] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyzhrhdrs.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvqvkrpkh.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/gjiittxnu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glzjzktlc.sHtML

[R26] 命令替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gxttwypxe.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fanxiaobao.xyz/Article/details/gmxdoawxz.sHtML

[R27] 算术展开
来源：http://m.share.fanxiaobao.xyz/Article/details/gicqeopdr.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fanxiaobao.xyz/Article/details/glyhbbmqv.sHtML

[R28] 浮点运算
来源：http://baike.fanxiaobao.xyz/Article/details/gyzzzcawx.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqhlfoctg.sHtML

[R29] 定义函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gftjrdmde.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fanxiaobao.xyz/Article/details/glshtfgej.sHtML

[R30] 函数返回状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gzqhfljwb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fanxiaobao.xyz/Article/details/gojronotb.sHtML

[R31] 局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/ggsefmptw.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gmpeqwspn.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzgfjejdh.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gdejeogql.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fanxiaobao.xyz/Article/details/geffsoovy.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fanxiaobao.xyz/Article/details/gzzfhjple.sHtML

[R34] 退出时清理
来源：http://blog.fanxiaobao.xyz/Article/details/gmisikzam.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gszplwpkg.sHtML

[R35] 后台执行并等待
来源：http://www.share.fanxiaobao.xyz/Article/details/giosodwhk.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fanxiaobao.xyz/Article/details/gjcqdkxru.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmirvxjct.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fanxiaobao.xyz/Article/details/gkhpfnjcf.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fanxiaobao.xyz/Article/details/guwwovcff.sHtML

files=$(ls -1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gitdpzmtk.sHtML

[R38] 管道串联
来源：http://read.share.fanxiaobao.xyz/Article/details/gwkkvvbix.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gfbnvnkvp.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gjpvkxgxx.sHtML

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gxrvqtlkz.sHtML

[R40] 追加写日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gsmgpyqwa.sHtML

echo "log" >> out.log
来源：http://read.share.fanxiaobao.xyz/Article/details/ghatsypax.sHtML

[R41] 丢弃输出
来源：http://blog.fanxiaobao.xyz/Article/details/gweiyqggw.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gziafdlia.sHtML

[R42] 输入重定向
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghpsmkjzp.sHtML

wc -l < a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gnccgwkmo.sHtML

[R43] 按名字查找文件
来源：http://blog.fanxiaobao.xyz/Article/details/glrozyexr.sHtML

find . -name "*.log" -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gityzdjvk.sHtML

[R44] 按修改时间查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gjtlvqjll.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvziagwio.sHtML

[R45] 批量删除
来源：http://blog.fanxiaobao.xyz/Article/details/gvztszfmv.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fanxiaobao.xyz/Article/details/gduervbnh.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fanxiaobao.xyz/Article/details/gktxtjauy.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtoievqxn.sHtML

[R47] sed 单行替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvjzffjof.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gdautkwcz.sHtML

[R48] awk 取指定列
来源：http://blog.fanxiaobao.xyz/Article/details/gbscvzdet.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/ghdwybgnk.sHtML

[R49] awk 带条件
来源：http://3g.fanxiaobao.xyz/Article/details/gfnduywqj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fanxiaobao.xyz/Article/details/grnzqcuoe.sHtML

[R50] awk 求和
来源：http://wap.fanxiaobao.xyz/Article/details/gspthkugr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/grnpgfzuq.sHtML

[R51] 排序去重取前几
来源：http://blog.fanxiaobao.xyz/Article/details/gedbnvybx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggoslstpj.sHtML

[R52] 统计行数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gouokyggv.sHtML

wc -l a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmvvzkjcm.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fanxiaobao.xyz/Article/details/gqwwttbcw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdtvfrhjy.sHtML

[R54] 比较两个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gizpqenrg.sHtML

diff a.txt b.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gkmbsoyup.sHtML

[R55] 压缩与解压
来源：http://m.share.fanxiaobao.xyz/Article/details/gvqgwdntu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fanxiaobao.xyz/Article/details/gfbgfxcpk.sHtML

[R56] 远程拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gltkzwfqu.sHtML

scp file user@host:/path/
来源：http://blog.fanxiaobao.xyz/Article/details/gcomngrqk.sHtML

[R57] 远程执行命令
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwxwfvgzk.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtnwvwkav.sHtML

[R58] 下载文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaofiscbo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fanxiaobao.xyz/Article/details/guctkhzsr.sHtML

[R59] 发 POST JSON
来源：http://wap.fanxiaobao.xyz/Article/details/glcpikgwl.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fanxiaobao.xyz/Article/details/glinbncwh.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gtkdzaspc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fanxiaobao.xyz/Article/details/gxmvnxfvs.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gszifobpc.sHtML

df -h;  du -sh *
来源：http://baike.fanxiaobao.xyz/Article/details/gvlunsbmk.sHtML

[R62] 找最占空间的文件
来源：http://3g.fanxiaobao.xyz/Article/details/ghbcoyuld.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gusqsxuhl.sHtML

[R63] 内存与进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gxhiqoqgr.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fanxiaobao.xyz/Article/details/ghbcivkxl.sHtML

[R64] 结束进程
来源：http://wap.fanxiaobao.xyz/Article/details/gvqyieoay.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fanxiaobao.xyz/Article/details/giccqmoee.sHtML

[R65] 查看端口占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gzuowrkjv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fanxiaobao.xyz/Article/details/gftelrpvl.sHtML

[R66] 定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/gqmwytfkz.sHtML

crontab -e;  crontab -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gkqebmhll.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fanxiaobao.xyz/Article/details/guqrteyos.sHtML

openssl rand -hex 16
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glrauibtr.sHtML

[R68] 计算文件校验值
来源：http://m.share.fanxiaobao.xyz/Article/details/gecodgwxt.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gmwwkfxvs.sHtML

[R69] 生成随机密码
来源：http://m.share.fanxiaobao.xyz/Article/details/gxzslcggg.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaflidvcb.sHtML

[R70] 时间戳与互转
来源：http://3g.fanxiaobao.xyz/Article/details/gbxlqujwx.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fanxiaobao.xyz/Article/details/gmmcqmmih.sHtML

[R71] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gildagikd.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fanxiaobao.xyz/Article/details/gupyjtmzd.sHtML

[R72] 等待端口就绪
来源：http://www.share.fanxiaobao.xyz/Article/details/gknzeahtk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gsrddcdlz.sHtML

[R73] 分割大日志
来源：http://wap.fanxiaobao.xyz/Article/details/gccftvlfk.sHtML

split -l 1000 big.log part_
来源：http://blog.fanxiaobao.xyz/Article/details/gblmdjqkk.sHtML

[R74] 批量重命名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gptrniwwj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfbttcieh.sHtML

[R75] 导出环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/glpvwtsfk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fanxiaobao.xyz/Article/details/gxnzaskct.sHtML

[R76] 使用临时文件
来源：http://m.share.fanxiaobao.xyz/Article/details/geevgqbzl.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gwcnslijc.sHtML

[R77] 读取用户输入
来源：http://baike.fanxiaobao.xyz/Article/details/gzlsdgcam.sHtML

read -rp "请输入: " ans
来源：http://blog.fanxiaobao.xyz/Article/details/gxcflbssj.sHtML

[R78] 交互式菜单
来源：http://read.share.fanxiaobao.xyz/Article/details/gvewutuck.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fanxiaobao.xyz/Article/details/gdzfbceht.sHtML

[R79] 解析命令行选项
来源：http://m.share.fanxiaobao.xyz/Article/details/geyyacapr.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwnychnkk.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fanxiaobao.xyz/Article/details/gwggehhgt.sHtML

time ./run.sh
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggzgqjizh.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gygnwszdu.sHtML

S. C / C++ 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gehurbuhp.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gtejmkdcw.sHtML

[S01] C：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gtwcovdhv.sHtML

#include <stdio.h>
来源：http://read.share.fanxiaobao.xyz/Article/details/gqmpcvovt.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fanxiaobao.xyz/Article/details/gdiuctbeg.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fanxiaobao.xyz/Article/details/geluzqlnw.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gcdkdfdmn.sHtML

[S03] C：读入整数
来源：http://3g.fanxiaobao.xyz/Article/details/gouontios.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gexkkevmh.sHtML

[S04] C：字符串复制
来源：http://www.share.fanxiaobao.xyz/Article/details/gbmblqejk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gttplstkj.sHtML

[S05] C：字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gsvxgvdsf.sHtML

strlen(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gdkiytxtc.sHtML

[S06] C：字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gsxhphlcb.sHtML

strcmp(a, b) == 0
来源：http://m.share.fanxiaobao.xyz/Article/details/ggtasmqnm.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbkcwybog.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fanxiaobao.xyz/Article/details/gmbzpeyij.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fanxiaobao.xyz/Article/details/gztqsvumj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fanxiaobao.xyz/Article/details/gmwufalgr.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fanxiaobao.xyz/Article/details/gsrbemecf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fanxiaobao.xyz/Article/details/ggdffpuix.sHtML

[S10] C：指针与解引用
来源：http://m.share.fanxiaobao.xyz/Article/details/gcbbuvxmt.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/garbftovq.sHtML

[S11] C：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gjnsozhum.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fanxiaobao.xyz/Article/details/gteimqvvi.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gneyawkjh.sHtML

fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gyxjebzdc.sHtML

[S12] C：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gjqipwcrb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/giqkivelu.sHtML

[S13] C：宏定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gtoosamzo.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghoqjrlss.sHtML

[S14] C：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gduccbnev.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fanxiaobao.xyz/Article/details/grcovlnmh.sHtML

[S15] C：类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gnsvzcnqr.sHtML

(double) a / b
来源：http://baike.fanxiaobao.xyz/Article/details/gejvxugip.sHtML

[S16] C：位操作置位
来源：http://www.share.fanxiaobao.xyz/Article/details/gyvzxkzto.sHtML

x |= (1 << 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gyueqygjt.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gtjujmwqo.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnomhjfxm.sHtML

[S18] C：命令行参数
来源：http://3g.fanxiaobao.xyz/Article/details/gdjxuttaf.sHtML

int main(int argc, char **argv)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdhvrvsab.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/gskvzxuxq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gpakogpkp.sHtML

[S20] C：二分查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmtjabpxz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzzybzpdg.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gypiggqtf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzzqicfca.sHtML

[S22] C：字符串转数字
来源：http://3g.fanxiaobao.xyz/Article/details/gbjcrawyx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/grnhrruoc.sHtML

[S23] C：随机数
来源：http://m.share.fanxiaobao.xyz/Article/details/gogovgxik.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjsoglvzw.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gckcfuapt.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fanxiaobao.xyz/Article/details/guchnqfqr.sHtML

[S25] C：内存拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gikrghorx.sHtML

memcpy(dst, src, n);
来源：http://baike.fanxiaobao.xyz/Article/details/gbtmggazk.sHtML

[S26] C：内存清零
来源：http://mobile.fanxiaobao.xyz/Article/details/gxndxqvcs.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fanxiaobao.xyz/Article/details/gcwonmnvr.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/gosllhnmj.sHtML

const double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtqptezjh.sHtML

[S28] C：静态变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/grpgcaqiw.sHtML

static int counter = 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/giqrgedee.sHtML

[S29] C：变参函数
来源：http://wap.fanxiaobao.xyz/Article/details/gdfbprjxe.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fanxiaobao.xyz/Article/details/gwreuchml.sHtML

[S30] C：头文件保护
来源：http://www.share.fanxiaobao.xyz/Article/details/gacntrgyh.sHtML

#ifndef X_H
来源：http://baike.fanxiaobao.xyz/Article/details/glicymsgo.sHtML

#define X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gbaponhvq.sHtML

#endif
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdalvjjp.sHtML

[S31] C++：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gstlvbmyj.sHtML

#include <iostream>
来源：http://3g.fanxiaobao.xyz/Article/details/goqabvozr.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbfraoye.sHtML

[S32] C++：字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gqdwohpoj.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fanxiaobao.xyz/Article/details/gjlidrkye.sHtML

[S33] C++：vector 增删
来源：http://www.share.fanxiaobao.xyz/Article/details/gfkaoazlm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gqwuhpark.sHtML

[S34] C++：遍历 vector
来源：http://3g.fanxiaobao.xyz/Article/details/guxqzlpcy.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhxkcfym.sHtML

[S35] C++：map
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtzwmgjg.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/glcatyltm.sHtML

[S36] C++：unordered_map
来源：http://mobile.fanxiaobao.xyz/Article/details/giglyhieb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/grymeeklc.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/gnuzxwdvx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbsqjgqlp.sHtML

[S38] C++：排序
来源：http://blog.fanxiaobao.xyz/Article/details/glcuiqlcc.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/ghldnrkch.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gukpcdrfu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fanxiaobao.xyz/Article/details/gokrbwxkw.sHtML

[S40] C++：查找元素
来源：http://wap.fanxiaobao.xyz/Article/details/gwpztzfeq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fanxiaobao.xyz/Article/details/ghyboqzhi.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdswfazem.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gbvukkdxg.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gslnjdvad.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fanxiaobao.xyz/Article/details/geupirjzh.sHtML

[S43] C++：智能指针
来源：http://blog.fanxiaobao.xyz/Article/details/gtylsqznq.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fanxiaobao.xyz/Article/details/gnqdgyino.sHtML

[S44] C++：引用传参
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaddfmqio.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gybjatqzx.sHtML

[S45] C++：lambda
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxtbgkpg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gestzchyk.sHtML

[S46] C++：函数模板
来源：http://wap.fanxiaobao.xyz/Article/details/gzsfqgpmu.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/guezzhnpr.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gyuzjjoiz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fanxiaobao.xyz/Article/details/gwriumswp.sHtML

[S48] C++：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gruzslsfs.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gepsrfauc.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdzyxdsff.sHtML

[S49] C++：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/ghqeodtzt.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/gaswlrqzz.sHtML

[S50] C++：格式化数字
来源：http://blog.fanxiaobao.xyz/Article/details/gghlhanvi.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzwotlmzj.sHtML

[S51] C++：显式类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gmqytbmmy.sHtML

static_cast<double>(a) / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gjvoyxloc.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fanxiaobao.xyz/Article/details/gsqagsepj.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzgkgvdip.sHtML

[S53] C++：移动语义
来源：http://3g.fanxiaobao.xyz/Article/details/gcotidxsw.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fanxiaobao.xyz/Article/details/gslxjiefu.sHtML

[S54] C++：异常处理
来源：http://mobile.fanxiaobao.xyz/Article/details/geujyorrf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gmtpdnzfw.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/ggnjamokq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fanxiaobao.xyz/Article/details/gradfraax.sHtML

[S56] C++：optional
来源：http://www.share.fanxiaobao.xyz/Article/details/gzqivhmof.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfltdlgmh.sHtML

[S57] C++：编译期常量
来源：http://wap.fanxiaobao.xyz/Article/details/gldbitthf.sHtML

constexpr int N = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/glijsvhnw.sHtML

[S58] C++：命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gupvezohu.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpvvmugjs.sHtML

[S59] C++：静态断言
来源：http://read.share.fanxiaobao.xyz/Article/details/gjepuvitn.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fanxiaobao.xyz/Article/details/glfcjkxij.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gtwphmaml.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gehooqoxi.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/glfinhrdc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fanxiaobao.xyz/Article/details/ghexltoel.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gqthhhjux.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gbgriiyjk.sHtML

println("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gqlkqnwap.sHtML

[T02] Kotlin：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gukqccpax.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fanxiaobao.xyz/Article/details/gkfmrtopb.sHtML


<!-- 参考信息 -->