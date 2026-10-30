代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gvzjrpcaw.sHtML

[R08] 数值比较
来源：http://wap.fanxiaobao.xyz/Article/details/gwbcywelg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/giorjemep.sHtML

[R09] 字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gdlfsdogk.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/grwbwylsb.sHtML

[R10] 正则匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpafxsdzh.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmizgocep.sHtML

[R11] case 多分支
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjbnpofe.sHtML

case "$1" in
来源：http://www.blog.fanxiaobao.xyz/Article/details/gujqgjxqb.sHtML

start) echo "启动" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvedksytx.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzbheaukd.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gssyxzyjm.sHtML

esac
来源：http://m.share.fanxiaobao.xyz/Article/details/gsuwshjhz.sHtML

[R12] for 遍历文件
来源：http://baike.fanxiaobao.xyz/Article/details/gjcqlwvnc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gymhpqobg.sHtML

[R13] for 计数循环
来源：http://blog.fanxiaobao.xyz/Article/details/gcxyzigwq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/glpcotyol.sHtML

[R14] C 风格 for
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwojyjfsv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gieqnfyfa.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gchqebyec.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/geuldcfzu.sHtML

[R16] until 等待条件
来源：http://wap.fanxiaobao.xyz/Article/details/gbzfqtgbm.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/godtoqkkd.sHtML

[R17] 数组定义与取值
来源：http://www.share.fanxiaobao.xyz/Article/details/gizhjmcuc.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdyihydxz.sHtML

[R18] 遍历数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gbbxnrbny.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gjvsbtkuy.sHtML

[R19] 数组长度
来源：http://wap.fanxiaobao.xyz/Article/details/gdjzhmyol.sHtML

echo "${#arr[@]}"
来源：http://blog.fanxiaobao.xyz/Article/details/guvckksue.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyycdvvmb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gsezcvtay.sHtML

[R21] 字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gexeswgic.sHtML

echo "${#s}"
来源：http://blog.fanxiaobao.xyz/Article/details/gssgrkmuz.sHtML

[R22] 截取子串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmpiffcm.sHtML

echo "${s:0:5}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gstbklrda.sHtML

[R23] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghcspqxzf.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gonnhuxlc.sHtML

[R24] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/grgbzdzlr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fanxiaobao.xyz/Article/details/gxtfiztcc.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fanxiaobao.xyz/Article/details/gacpnukyu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gieywrtbs.sHtML

[R26] 命令替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gfqgezoyp.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghemokzmz.sHtML

[R27] 算术展开
来源：http://read.share.fanxiaobao.xyz/Article/details/gvpfxpepj.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fanxiaobao.xyz/Article/details/gijmjxpiw.sHtML

[R28] 浮点运算
来源：http://wap.fanxiaobao.xyz/Article/details/gvmalqbdn.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fanxiaobao.xyz/Article/details/glcfunjhm.sHtML

[R29] 定义函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxxolpdbb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gerfzjskl.sHtML

[R30] 函数返回状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gboxytkze.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fanxiaobao.xyz/Article/details/gqcvgfryb.sHtML

[R31] 局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsqcdhsvc.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gprozsyly.sHtML

[R32] 参数个数校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gryquweer.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghappoluz.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gcherzolx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fanxiaobao.xyz/Article/details/grwghcdxs.sHtML

[R34] 退出时清理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhvxhdre.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/geakhlibn.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqzuzxclt.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fanxiaobao.xyz/Article/details/gigylfink.sHtML

[R36] 并发执行多个任务
来源：http://blog.fanxiaobao.xyz/Article/details/gocrpttdx.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyycmqafp.sHtML

[R37] 把输出赋给变量
来源：http://baike.fanxiaobao.xyz/Article/details/gezxhiute.sHtML

files=$(ls -1)
来源：http://baike.fanxiaobao.xyz/Article/details/gvxsoysck.sHtML

[R38] 管道串联
来源：http://3g.fanxiaobao.xyz/Article/details/gjkyjztwz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fanxiaobao.xyz/Article/details/grnwlrvkh.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fanxiaobao.xyz/Article/details/gwqldlabh.sHtML

cmd > out.log 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/grdvloavc.sHtML

[R40] 追加写日志
来源：http://wap.fanxiaobao.xyz/Article/details/gjljrqiul.sHtML

echo "log" >> out.log
来源：http://blog.fanxiaobao.xyz/Article/details/gbjhubkly.sHtML

[R41] 丢弃输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gagvsvpec.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gkipflhma.sHtML

[R42] 输入重定向
来源：http://m.share.fanxiaobao.xyz/Article/details/ghmapxnxg.sHtML

wc -l < a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzvgppvfy.sHtML

[R43] 按名字查找文件
来源：http://wap.fanxiaobao.xyz/Article/details/gvzimmpwc.sHtML

find . -name "*.log" -type f
来源：http://wap.fanxiaobao.xyz/Article/details/grggppbfy.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxpfpfab.sHtML

find . -mtime -7 -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gpslwpfgw.sHtML

[R45] 批量删除
来源：http://blog.fanxiaobao.xyz/Article/details/gewfjmpnu.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fanxiaobao.xyz/Article/details/gcypzvaov.sHtML

[R46] 递归替换文件内容
来源：http://wap.fanxiaobao.xyz/Article/details/gujgegfcd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fanxiaobao.xyz/Article/details/gcpclvgjw.sHtML

[R47] sed 单行替换
来源：http://baike.fanxiaobao.xyz/Article/details/gfqimmsjq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnqcflqkq.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gvrjsavjl.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshzykkbg.sHtML

[R49] awk 带条件
来源：http://wap.fanxiaobao.xyz/Article/details/gkokcsdgq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/gnjmycmcj.sHtML

[R50] awk 求和
来源：http://wap.fanxiaobao.xyz/Article/details/grhpxeeys.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmxnxbes.sHtML

[R51] 排序去重取前几
来源：http://mobile.fanxiaobao.xyz/Article/details/gqeghfblh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqmqfnvnq.sHtML

[R52] 统计行数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gibwjybwu.sHtML

wc -l a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggwjjvlsm.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fanxiaobao.xyz/Article/details/gvftbfbmx.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fanxiaobao.xyz/Article/details/gxjbiatxz.sHtML

[R54] 比较两个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzajoyppq.sHtML

diff a.txt b.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gmkxjlzgf.sHtML

[R55] 压缩与解压
来源：http://baike.fanxiaobao.xyz/Article/details/gwmxlblnl.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fanxiaobao.xyz/Article/details/gcfiablcd.sHtML

[R56] 远程拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfwrhywn.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/gfpihzzbe.sHtML

[R57] 远程执行命令
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzpwlgcz.sHtML

ssh user@host 'uptime'
来源：http://m.share.fanxiaobao.xyz/Article/details/guizcoyhw.sHtML

[R58] 下载文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gupceimvn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fanxiaobao.xyz/Article/details/gmxmqfyem.sHtML

[R59] 发 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/gkerivrpt.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fanxiaobao.xyz/Article/details/ghzeknrda.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gmnztdpyl.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaixoktph.sHtML

[R61] 磁盘占用
来源：http://blog.fanxiaobao.xyz/Article/details/glsjeiqcc.sHtML

df -h;  du -sh *
来源：http://baike.fanxiaobao.xyz/Article/details/ggdknqkwx.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggknhqers.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzwcsjbzh.sHtML

[R63] 内存与进程
来源：http://baike.fanxiaobao.xyz/Article/details/gqzqbtmly.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkdyzlypx.sHtML

[R64] 结束进程
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxlgesax.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmvcjnzde.sHtML

[R65] 查看端口占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdscflqmd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fanxiaobao.xyz/Article/details/gzulygewk.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gtmmasdvr.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gudyavtpb.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fanxiaobao.xyz/Article/details/gdrcynaxu.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/gprwfbkcs.sHtML

[R68] 计算文件校验值
来源：http://read.share.fanxiaobao.xyz/Article/details/gsucmrdic.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/grvdueqau.sHtML

[R69] 生成随机密码
来源：http://read.share.fanxiaobao.xyz/Article/details/gnnclgxpr.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fanxiaobao.xyz/Article/details/gxsmoekif.sHtML

[R70] 时间戳与互转
来源：http://m.share.fanxiaobao.xyz/Article/details/geoaqkjvd.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/gksjonxww.sHtML

[R71] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gbgkajdqf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fanxiaobao.xyz/Article/details/gwqvsbqwe.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/gebkmjaqj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/geplgiiek.sHtML

[R73] 分割大日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjaodynu.sHtML

split -l 1000 big.log part_
来源：http://www.share.fanxiaobao.xyz/Article/details/goucuyyjc.sHtML

[R74] 批量重命名
来源：http://www.share.fanxiaobao.xyz/Article/details/gjjpujgfa.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfwboopd.sHtML

[R75] 导出环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gzstdxocu.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fanxiaobao.xyz/Article/details/gqhgwpmgi.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grtmeqafd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbrkotcnn.sHtML

[R77] 读取用户输入
来源：http://m.share.fanxiaobao.xyz/Article/details/ghyoyzcoq.sHtML

read -rp "请输入: " ans
来源：http://wap.fanxiaobao.xyz/Article/details/gmnpvtrzn.sHtML

[R78] 交互式菜单
来源：http://wap.fanxiaobao.xyz/Article/details/gvmgwdcmp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gfrzgsays.sHtML

[R79] 解析命令行选项
来源：http://blog.fanxiaobao.xyz/Article/details/gybucjakg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fanxiaobao.xyz/Article/details/gprjkfvtv.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/gcxfaxpwd.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/grqulpkay.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwpqxxdj.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gjyudqlaq.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gauegevgq.sHtML

[S01] C：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gboydjufv.sHtML

#include <stdio.h>
来源：http://www.share.fanxiaobao.xyz/Article/details/gpxerkphm.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gktgmhyoo.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fanxiaobao.xyz/Article/details/gsxladrtj.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fanxiaobao.xyz/Article/details/ggkxucznu.sHtML

[S03] C：读入整数
来源：http://3g.fanxiaobao.xyz/Article/details/gdklybdlh.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwdvmtrvd.sHtML

[S04] C：字符串复制
来源：http://read.share.fanxiaobao.xyz/Article/details/ggfvcsiyl.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtcpwqeqx.sHtML

[S05] C：字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxfstejt.sHtML

strlen(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtedjtkbh.sHtML

[S06] C：字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gqtclylss.sHtML

strcmp(a, b) == 0
来源：http://read.share.fanxiaobao.xyz/Article/details/gecurfmal.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqioabpev.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fanxiaobao.xyz/Article/details/gqebetsml.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fanxiaobao.xyz/Article/details/geyrapbuv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwyavrnog.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fanxiaobao.xyz/Article/details/guujbalub.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fanxiaobao.xyz/Article/details/grcpelelu.sHtML

[S10] C：指针与解引用
来源：http://read.share.fanxiaobao.xyz/Article/details/gxxmwxcsl.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/gasibaxyn.sHtML

[S11] C：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/ghvdlwwpj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvxthzny.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggnbulmps.sHtML

fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gxbplswmf.sHtML

[S12] C：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gznvaegeo.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/grfvwbgjv.sHtML

[S13] C：宏定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gjllkbtqi.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fanxiaobao.xyz/Article/details/goihnadps.sHtML

[S14] C：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gxaumyvsk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fanxiaobao.xyz/Article/details/gwybswwrj.sHtML

[S15] C：类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/glppaouqp.sHtML

(double) a / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/griyryviz.sHtML

[S16] C：位操作置位
来源：http://blog.fanxiaobao.xyz/Article/details/gxboacyhm.sHtML

x |= (1 << 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvxolfhct.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gdgrgvvmo.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fanxiaobao.xyz/Article/details/gvnbajelq.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gzeyzqoia.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gomtqiabq.sHtML

[S19] C：快速排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gowulgamo.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gxwdtdexv.sHtML

[S20] C：二分查找
来源：http://wap.fanxiaobao.xyz/Article/details/gzbwyhcdw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghkpcdhzz.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/gpmskhwuh.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkspphdrk.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/gwnqjzutn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/gzqzsecyg.sHtML

[S23] C：随机数
来源：http://3g.fanxiaobao.xyz/Article/details/gazgjibio.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gnrgmgzrb.sHtML

[S24] C：获取本地时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gmgdcsgoq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fanxiaobao.xyz/Article/details/gurrsxmeg.sHtML

[S25] C：内存拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gnoalaavd.sHtML

memcpy(dst, src, n);
来源：http://blog.fanxiaobao.xyz/Article/details/gxzgzbnch.sHtML

[S26] C：内存清零
来源：http://read.share.fanxiaobao.xyz/Article/details/glfoxwhvr.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fanxiaobao.xyz/Article/details/glccknfpb.sHtML

[S27] C：定义常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmcwriplt.sHtML

const double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gckyoyujb.sHtML

[S28] C：静态变量
来源：http://3g.fanxiaobao.xyz/Article/details/gdzayosmy.sHtML

static int counter = 0;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggkocrxth.sHtML

[S29] C：变参函数
来源：http://baike.fanxiaobao.xyz/Article/details/gtudnvfll.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbhpxpzyw.sHtML

[S30] C：头文件保护
来源：http://blog.fanxiaobao.xyz/Article/details/gmtxznvwz.sHtML

#ifndef X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gpshxxzjt.sHtML

#define X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjmpgoly.sHtML

#endif
来源：http://www.share.fanxiaobao.xyz/Article/details/gsigoitws.sHtML

[S31] C++：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gzehzsayu.sHtML

#include <iostream>
来源：http://blog.fanxiaobao.xyz/Article/details/govkowrev.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjlfvpcx.sHtML

[S32] C++：字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/ggpnvcawn.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjuokxts.sHtML

[S33] C++：vector 增删
来源：http://read.share.fanxiaobao.xyz/Article/details/gvwfeoikh.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gccxljifo.sHtML

[S34] C++：遍历 vector
来源：http://wap.fanxiaobao.xyz/Article/details/gvundfhxx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbessunvk.sHtML

[S35] C++：map
来源：http://www.share.fanxiaobao.xyz/Article/details/gkagjfcyc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/ghzukjbsj.sHtML

[S36] C++：unordered_map
来源：http://blog.fanxiaobao.xyz/Article/details/ghavshegf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gwrkdhuyb.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/ghopcfonw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvyilyead.sHtML

[S38] C++：排序
来源：http://blog.fanxiaobao.xyz/Article/details/gdfugbhaq.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gczikszrv.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fanxiaobao.xyz/Article/details/ggvlnpsqx.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fanxiaobao.xyz/Article/details/gavzxndct.sHtML

[S40] C++：查找元素
来源：http://www.share.fanxiaobao.xyz/Article/details/ghacyhevt.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gzsihydjr.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gidateboa.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gmdufhysg.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fanxiaobao.xyz/Article/details/gccrefwzg.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwmtvcxb.sHtML

[S43] C++：智能指针
来源：http://3g.fanxiaobao.xyz/Article/details/gbtketklk.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvexvvvg.sHtML

[S44] C++：引用传参
来源：http://mobile.fanxiaobao.xyz/Article/details/gsavjyivm.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gwosbsgei.sHtML

[S45] C++：lambda
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grawakcxj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fanxiaobao.xyz/Article/details/ggiuvtojv.sHtML

[S46] C++：函数模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gzfkavpfa.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gyrwskdgj.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzlkkiaik.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fanxiaobao.xyz/Article/details/govjazulp.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gockbkhut.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdtaveur.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghiiudalq.sHtML

[S49] C++：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/grlgmrqnx.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geyvgqrwi.sHtML

[S50] C++：格式化数字
来源：http://3g.fanxiaobao.xyz/Article/details/gufmkyxje.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gqojulrme.sHtML

[S51] C++：显式类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gcxvwpvuc.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvmpgdafi.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fanxiaobao.xyz/Article/details/gyqfpnlmw.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnymnzyql.sHtML

[S53] C++：移动语义
来源：http://read.share.fanxiaobao.xyz/Article/details/gpylaubxe.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fanxiaobao.xyz/Article/details/gggbcfbrl.sHtML

[S54] C++：异常处理
来源：http://baike.fanxiaobao.xyz/Article/details/gskzzhojm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvvtpfazn.sHtML

[S55] C++：结构化绑定
来源：http://3g.fanxiaobao.xyz/Article/details/gcbytfpsh.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkwmsfikn.sHtML

[S56] C++：optional
来源：http://www.share.fanxiaobao.xyz/Article/details/gqezonjlo.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fanxiaobao.xyz/Article/details/gpjzduuzo.sHtML

[S57] C++：编译期常量
来源：http://blog.fanxiaobao.xyz/Article/details/goyftbhdu.sHtML

constexpr int N = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/grqnxnzqi.sHtML

[S58] C++：命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/gzdxueipo.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfqifzwmt.sHtML

[S59] C++：静态断言
来源：http://m.share.fanxiaobao.xyz/Article/details/gloouxivw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fanxiaobao.xyz/Article/details/ggemjdbrj.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fanxiaobao.xyz/Article/details/gshtxnnlp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyjzuklmq.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkihwpofz.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fanxiaobao.xyz/Article/details/gfunpatqq.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfxvctfm.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmxsenmt.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gaekfpitj.sHtML

[T02] Kotlin：变量
来源：http://blog.fanxiaobao.xyz/Article/details/gquqhupgn.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fanxiaobao.xyz/Article/details/gxdinzvae.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkdpebytt.sHtML

"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/glgwwcrak.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fanxiaobao.xyz/Article/details/gukqpfzak.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gliyfztjv.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gfvxjjyhg.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fanxiaobao.xyz/Article/details/grzdmpxvn.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/gbfrloupv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfctpjbak.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gjxktisrz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyqfavrjk.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/gjjkntydh.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/gxcqzzqjb.sHtML


<!-- 参考信息 -->