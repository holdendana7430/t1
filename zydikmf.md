代发 wailian999

readonly PI=3.14
来源：http://mobile.hesvh.cn/Article/details/gbrzslwlc.sHtML

[R04] 位置参数
来源：http://www.m.share.fehbvm.com/Article/details/ghsyiuiak.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.zdbjq.cn/Article/details/gppexmxne.sHtML

[R05] 参数默认值
来源：http://blog.fehbvm.com/Article/details/gbtzjsqoq.sHtML

name="${1:-default}"
来源：http://www.m.share.zdbjq.cn/Article/details/gjazmculs.sHtML

[R06] 判断命令是否存在
来源：http://3g.fehbvm.com/Article/details/gwootmtsr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/gjipadbyl.sHtML

[R07] if 判断文件
来源：http://mobile.zdbjq.cn/Article/details/glbosippp.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.zdbjq.cn/Article/details/gmaxnnrqw.sHtML

[R08] 数值比较
来源：http://mobile.fehbvm.com/Article/details/gvzpdyyrz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.zdbjq.cn/Article/details/glcccbwvm.sHtML

[R09] 字符串比较
来源：http://3g.hesvh.cn/Article/details/gtkqppxbl.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gehzptofi.sHtML

[R10] 正则匹配
来源：http://3g.hesvh.cn/Article/details/gmxldnlyb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.hesvh.cn/Article/details/gjtwtinkd.sHtML

[R11] case 多分支
来源：http://m.share.zdbjq.cn/Article/details/gyvrsfcte.sHtML

case "$1" in
来源：http://www.blog.hesvh.cn/Article/details/gkzejztgp.sHtML

start) echo "启动" ;;
来源：http://baike.fehbvm.com/Article/details/gqluyyikh.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.hesvh.cn/Article/details/gcfjucogu.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fehbvm.com/Article/details/gxguvfley.sHtML

esac
来源：http://mobile.zdbjq.cn/Article/details/gaavwuibp.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fehbvm.com/Article/details/gztkamall.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.zdbjq.cn/Article/details/gsfmcukxa.sHtML

[R13] for 计数循环
来源：http://wap.zdbjq.cn/Article/details/gdsybfxtl.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/gugjrcruk.sHtML

[R14] C 风格 for
来源：http://blog.zdbjq.cn/Article/details/gvikwhhjg.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/gjfbnyvoi.sHtML

[R15] while 逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gwbgsrqjk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.zdbjq.cn/Article/details/gdzohsalu.sHtML

[R16] until 等待条件
来源：http://blog.zdbjq.cn/Article/details/gdbfrbafv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/gptbtrgkx.sHtML

[R17] 数组定义与取值
来源：http://www.share.fehbvm.com/Article/details/gdytxiobt.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fehbvm.com/Article/details/gulpaznkx.sHtML

[R18] 遍历数组
来源：http://www.m.share.fehbvm.com/Article/details/gvdficdue.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.zdbjq.cn/Article/details/golttnjug.sHtML

[R19] 数组长度
来源：http://www.blog.zdbjq.cn/Article/details/gxszdivne.sHtML

echo "${#arr[@]}"
来源：http://read.share.hesvh.cn/Article/details/gzmgguskw.sHtML

[R20] 关联数组（字典）
来源：http://blog.zdbjq.cn/Article/details/gvdmxlryu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.hesvh.cn/Article/details/gdmppxtdv.sHtML

[R21] 字符串长度
来源：http://www.share.hesvh.cn/Article/details/glscrfmww.sHtML

echo "${#s}"
来源：http://3g.hesvh.cn/Article/details/gvizrsplf.sHtML

[R22] 截取子串
来源：http://blog.zdbjq.cn/Article/details/goznxblgg.sHtML

echo "${s:0:5}"
来源：http://m.share.hesvh.cn/Article/details/gypfoxqxr.sHtML

[R23] 字符串替换
来源：http://mobile.zdbjq.cn/Article/details/gwzvsdgaf.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.zdbjq.cn/Article/details/gdhfdwmqo.sHtML

[R24] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/gebrwlvxo.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.hesvh.cn/Article/details/gdutjhdyr.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fehbvm.com/Article/details/gjdrsfcbu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.zdbjq.cn/Article/details/gxvxazaef.sHtML

[R26] 命令替换
来源：http://wap.zdbjq.cn/Article/details/gpwvvlnpc.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fehbvm.com/Article/details/gqrabadni.sHtML

[R27] 算术展开
来源：http://www.m.share.fehbvm.com/Article/details/gnuyeuijd.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.hesvh.cn/Article/details/gdbspbnlo.sHtML

[R28] 浮点运算
来源：http://wap.fehbvm.com/Article/details/ghusbsepj.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.zdbjq.cn/Article/details/gfmzykgpp.sHtML

[R29] 定义函数
来源：http://www.blog.hesvh.cn/Article/details/graljctky.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fehbvm.com/Article/details/guyoqnlsf.sHtML

[R30] 函数返回状态码
来源：http://m.share.hesvh.cn/Article/details/glbjgpprt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.hesvh.cn/Article/details/gimwrlfmx.sHtML

[R31] 局部变量
来源：http://wap.fehbvm.com/Article/details/gnxkbnxuc.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gollmhrjo.sHtML

[R32] 参数个数校验
来源：http://www.m.share.zdbjq.cn/Article/details/gognhqfyo.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/gmshfgvyp.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.zdbjq.cn/Article/details/gfbhdgpev.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fehbvm.com/Article/details/gsfkmzfne.sHtML

[R34] 退出时清理
来源：http://www.m.share.hesvh.cn/Article/details/ggmjzygbv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/ggzwdpdkr.sHtML

[R35] 后台执行并等待
来源：http://wap.hesvh.cn/Article/details/gihzplyzi.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.zdbjq.cn/Article/details/gijyrhxip.sHtML

[R36] 并发执行多个任务
来源：http://baike.zdbjq.cn/Article/details/gmkucumwu.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.zdbjq.cn/Article/details/gcjjeiqrc.sHtML

[R37] 把输出赋给变量
来源：http://3g.zdbjq.cn/Article/details/gppanftid.sHtML

files=$(ls -1)
来源：http://www.blog.zdbjq.cn/Article/details/gwppbzygh.sHtML

[R38] 管道串联
来源：http://mobile.fehbvm.com/Article/details/gjfusoyye.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.hesvh.cn/Article/details/gydgqnrsf.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fehbvm.com/Article/details/gdcqysqgw.sHtML

cmd > out.log 2>&1
来源：http://mobile.hesvh.cn/Article/details/ghokfjcfu.sHtML

[R40] 追加写日志
来源：http://mobile.fehbvm.com/Article/details/gzfakuegh.sHtML

echo "log" >> out.log
来源：http://read.share.hesvh.cn/Article/details/gksurrwax.sHtML

[R41] 丢弃输出
来源：http://read.share.hesvh.cn/Article/details/gvlnjewdk.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.zdbjq.cn/Article/details/geaqrbjvl.sHtML

[R42] 输入重定向
来源：http://read.share.fehbvm.com/Article/details/gwtumieud.sHtML

wc -l < a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gjalpjdke.sHtML

[R43] 按名字查找文件
来源：http://m.share.zdbjq.cn/Article/details/gpnfjtyel.sHtML

find . -name "*.log" -type f
来源：http://baike.fehbvm.com/Article/details/glrzjqwkj.sHtML

[R44] 按修改时间查找
来源：http://m.share.hesvh.cn/Article/details/guwzdwipc.sHtML

find . -mtime -7 -type f
来源：http://baike.fehbvm.com/Article/details/gcstmndvq.sHtML

[R45] 批量删除
来源：http://baike.fehbvm.com/Article/details/ganjohary.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.hesvh.cn/Article/details/gynqkuxbf.sHtML

[R46] 递归替换文件内容
来源：http://wap.fehbvm.com/Article/details/gezjfpmka.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fehbvm.com/Article/details/ggeddhecb.sHtML

[R47] sed 单行替换
来源：http://wap.fehbvm.com/Article/details/gppfbguqk.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gddsbrwlk.sHtML

[R48] awk 取指定列
来源：http://blog.fehbvm.com/Article/details/gaxzisuda.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gmxtyovzn.sHtML

[R49] awk 带条件
来源：http://read.share.zdbjq.cn/Article/details/gsfgyfkzu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.zdbjq.cn/Article/details/gytqpvsep.sHtML

[R50] awk 求和
来源：http://www.share.fehbvm.com/Article/details/grhsntlng.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fehbvm.com/Article/details/gkeddlbuz.sHtML

[R51] 排序去重取前几
来源：http://blog.hesvh.cn/Article/details/glphfgajt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.hesvh.cn/Article/details/gwbstgoji.sHtML

[R52] 统计行数
来源：http://mobile.fehbvm.com/Article/details/gipizpbsq.sHtML

wc -l a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/guwrgkhpz.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.zdbjq.cn/Article/details/gbguvrlvo.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.zdbjq.cn/Article/details/gcpjosste.sHtML

[R54] 比较两个文件
来源：http://read.share.fehbvm.com/Article/details/gziuvzuqs.sHtML

diff a.txt b.txt
来源：http://m.share.fehbvm.com/Article/details/gdpxfzbch.sHtML

[R55] 压缩与解压
来源：http://mobile.zdbjq.cn/Article/details/godxlzeld.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fehbvm.com/Article/details/gfizhztwd.sHtML

[R56] 远程拷贝
来源：http://baike.hesvh.cn/Article/details/gpreuffif.sHtML

scp file user@host:/path/
来源：http://3g.zdbjq.cn/Article/details/gxkowzorh.sHtML

[R57] 远程执行命令
来源：http://www.blog.zdbjq.cn/Article/details/gxvmfwddt.sHtML

ssh user@host 'uptime'
来源：http://read.share.hesvh.cn/Article/details/gueswojps.sHtML

[R58] 下载文件
来源：http://baike.fehbvm.com/Article/details/ghsoammss.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.hesvh.cn/Article/details/geehkexft.sHtML

[R59] 发 POST JSON
来源：http://blog.fehbvm.com/Article/details/gwsufxxiv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.zdbjq.cn/Article/details/gdbqfnvvb.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.hesvh.cn/Article/details/gwmicirua.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.hesvh.cn/Article/details/gmnzoavtn.sHtML

[R61] 磁盘占用
来源：http://wap.zdbjq.cn/Article/details/giricmirp.sHtML

df -h;  du -sh *
来源：http://3g.zdbjq.cn/Article/details/glpiisgts.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.zdbjq.cn/Article/details/gyxqpkxrj.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.hesvh.cn/Article/details/glhvdwydr.sHtML

[R63] 内存与进程
来源：http://wap.hesvh.cn/Article/details/gaezdpnwa.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.hesvh.cn/Article/details/gcqfcsmic.sHtML

[R64] 结束进程
来源：http://baike.zdbjq.cn/Article/details/gxioqatdw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.zdbjq.cn/Article/details/gffrsyxfp.sHtML

[R65] 查看端口占用
来源：http://m.share.fehbvm.com/Article/details/gvunmjxgw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.hesvh.cn/Article/details/gmqvrigzt.sHtML

[R66] 定时任务
来源：http://3g.hesvh.cn/Article/details/gqsteqsjh.sHtML

crontab -e;  crontab -l
来源：http://mobile.zdbjq.cn/Article/details/gyvhltukz.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.hesvh.cn/Article/details/gefzebdhy.sHtML

openssl rand -hex 16
来源：http://www.share.hesvh.cn/Article/details/gmfgqnjff.sHtML

[R68] 计算文件校验值
来源：http://www.share.zdbjq.cn/Article/details/gdktpiggv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gxvjcsygq.sHtML

[R69] 生成随机密码
来源：http://www.share.zdbjq.cn/Article/details/gjibwfwea.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.hesvh.cn/Article/details/goqvabuuz.sHtML

[R70] 时间戳与互转
来源：http://mobile.hesvh.cn/Article/details/gttdiawiu.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.zdbjq.cn/Article/details/gldtmoxng.sHtML

[R71] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gcolbaknh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.zdbjq.cn/Article/details/gyuxpqftt.sHtML

[R72] 等待端口就绪
来源：http://wap.zdbjq.cn/Article/details/gjmetcjqj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/gpucqrrcg.sHtML

[R73] 分割大日志
来源：http://www.m.share.zdbjq.cn/Article/details/gefkbyzoy.sHtML

split -l 1000 big.log part_
来源：http://mobile.zdbjq.cn/Article/details/gxgyllwrl.sHtML

[R74] 批量重命名
来源：http://baike.hesvh.cn/Article/details/gpasanpfz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.hesvh.cn/Article/details/gbdsuomat.sHtML

[R75] 导出环境变量
来源：http://m.share.hesvh.cn/Article/details/gajawtwin.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fehbvm.com/Article/details/gaydavdvp.sHtML

[R76] 使用临时文件
来源：http://www.blog.zdbjq.cn/Article/details/gkqkccsob.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.hesvh.cn/Article/details/gsruhvagg.sHtML

[R77] 读取用户输入
来源：http://m.share.fehbvm.com/Article/details/gpegydhyd.sHtML

read -rp "请输入: " ans
来源：http://baike.zdbjq.cn/Article/details/gfmsihjzx.sHtML

[R78] 交互式菜单
来源：http://www.blog.zdbjq.cn/Article/details/gqmlvqpao.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fehbvm.com/Article/details/gmpnhssgm.sHtML

[R79] 解析命令行选项
来源：http://wap.fehbvm.com/Article/details/grlmodnqx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.hesvh.cn/Article/details/gthocytxp.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fehbvm.com/Article/details/gtgdcdfkc.sHtML

time ./run.sh
来源：http://www.share.zdbjq.cn/Article/details/gyvbapuxg.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gmfmhypgq.sHtML

S. C / C++ 专题
来源：http://wap.hesvh.cn/Article/details/gocqbleaz.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gqcewbuhf.sHtML

[S01] C：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gsfokytno.sHtML

#include <stdio.h>
来源：http://www.blog.hesvh.cn/Article/details/groxtcawu.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fehbvm.com/Article/details/gaijcgzlc.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.zdbjq.cn/Article/details/gsaitbycr.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fehbvm.com/Article/details/ggisyhltl.sHtML

[S03] C：读入整数
来源：http://3g.zdbjq.cn/Article/details/gjpqlmwxh.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.zdbjq.cn/Article/details/gffhccest.sHtML

[S04] C：字符串复制
来源：http://baike.hesvh.cn/Article/details/ghqpeosuo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fehbvm.com/Article/details/gsyfbsbti.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/gwpxjfvok.sHtML

strlen(s)
来源：http://mobile.zdbjq.cn/Article/details/gibkvcxow.sHtML

[S06] C：字符串比较
来源：http://www.share.hesvh.cn/Article/details/gqmdjllyj.sHtML

strcmp(a, b) == 0
来源：http://www.blog.zdbjq.cn/Article/details/gqxtuuiob.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.hesvh.cn/Article/details/gmcusfjlx.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.zdbjq.cn/Article/details/guaopzjcf.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.zdbjq.cn/Article/details/giajhiuba.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fehbvm.com/Article/details/gqvzwctph.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fehbvm.com/Article/details/ggrkpatwb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.hesvh.cn/Article/details/gqqronaty.sHtML

[S10] C：指针与解引用
来源：http://read.share.fehbvm.com/Article/details/gayzfreqi.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fehbvm.com/Article/details/gyirrerty.sHtML

[S11] C：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gcwbwaswe.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.zdbjq.cn/Article/details/gdnurldld.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fehbvm.com/Article/details/gcdpnqnjw.sHtML

fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gffrlszqc.sHtML

[S12] C：写文件
来源：http://m.share.fehbvm.com/Article/details/guwadwrzb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/godtfafey.sHtML

[S13] C：宏定义
来源：http://www.share.hesvh.cn/Article/details/gyzvatigq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.zdbjq.cn/Article/details/gyfdpgvpf.sHtML

[S14] C：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gisxcqwmd.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.hesvh.cn/Article/details/grehahyph.sHtML

[S15] C：类型转换
来源：http://m.share.zdbjq.cn/Article/details/grgxkoram.sHtML

(double) a / b
来源：http://mobile.fehbvm.com/Article/details/gvabomjlu.sHtML

[S16] C：位操作置位
来源：http://www.share.hesvh.cn/Article/details/grmfgjtou.sHtML

x |= (1 << 3);
来源：http://baike.fehbvm.com/Article/details/gowbxzizm.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fehbvm.com/Article/details/gwfhkzsst.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.zdbjq.cn/Article/details/gwifdjwgr.sHtML

[S18] C：命令行参数
来源：http://wap.zdbjq.cn/Article/details/guyfqqada.sHtML

int main(int argc, char **argv)
来源：http://www.share.hesvh.cn/Article/details/gssnyfgdb.sHtML

[S19] C：快速排序
来源：http://www.share.hesvh.cn/Article/details/gfcvgqyhh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/gbfwerutl.sHtML

[S20] C：二分查找
来源：http://3g.fehbvm.com/Article/details/guphyvqna.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/gbiehmafj.sHtML

[S21] C：字符类别判断
来源：http://read.share.fehbvm.com/Article/details/gpeusykyv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.hesvh.cn/Article/details/guqqwkvwb.sHtML

[S22] C：字符串转数字
来源：http://m.share.fehbvm.com/Article/details/gyvtxdgcp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.hesvh.cn/Article/details/gcjesopmf.sHtML

[S23] C：随机数
来源：http://www.share.fehbvm.com/Article/details/gbepktlwc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.zdbjq.cn/Article/details/gsolrutvj.sHtML

[S24] C：获取本地时间
来源：http://mobile.zdbjq.cn/Article/details/gzfhzdllg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fehbvm.com/Article/details/gjaahwfbx.sHtML

[S25] C：内存拷贝
来源：http://baike.fehbvm.com/Article/details/gfzsnqrla.sHtML

memcpy(dst, src, n);
来源：http://baike.zdbjq.cn/Article/details/grbttbhro.sHtML

[S26] C：内存清零
来源：http://www.m.share.hesvh.cn/Article/details/gnnponzdn.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.hesvh.cn/Article/details/gixtuceoj.sHtML

[S27] C：定义常量
来源：http://3g.hesvh.cn/Article/details/gkfcjmgin.sHtML

const double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/glqanpvbi.sHtML

[S28] C：静态变量
来源：http://www.share.zdbjq.cn/Article/details/gxlphdsfq.sHtML

static int counter = 0;
来源：http://wap.hesvh.cn/Article/details/giuxbdklp.sHtML

[S29] C：变参函数
来源：http://blog.fehbvm.com/Article/details/gxphpgwlx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.zdbjq.cn/Article/details/gptqmlbuv.sHtML

[S30] C：头文件保护
来源：http://baike.fehbvm.com/Article/details/gziyxfxgv.sHtML

#ifndef X_H
来源：http://wap.fehbvm.com/Article/details/gmipatlpd.sHtML

#define X_H
来源：http://www.share.hesvh.cn/Article/details/gbrrmwcly.sHtML

#endif
来源：http://m.share.zdbjq.cn/Article/details/gjfrdjgdq.sHtML

[S31] C++：Hello World
来源：http://baike.fehbvm.com/Article/details/gcomhlhiv.sHtML

#include <iostream>
来源：http://m.share.hesvh.cn/Article/details/gzmsimzcr.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fehbvm.com/Article/details/gxzycpbon.sHtML

[S32] C++：字符串
来源：http://wap.zdbjq.cn/Article/details/glqghzahc.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.zdbjq.cn/Article/details/gnaffwadz.sHtML

[S33] C++：vector 增删
来源：http://mobile.fehbvm.com/Article/details/gxeqhgvkd.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gpyrygtqp.sHtML

[S34] C++：遍历 vector
来源：http://baike.zdbjq.cn/Article/details/gskizdzfj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdekxddnk.sHtML

[S35] C++：map
来源：http://blog.zdbjq.cn/Article/details/ggrwxofhl.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/gsgnalqpv.sHtML

[S36] C++：unordered_map
来源：http://3g.hesvh.cn/Article/details/goromplyi.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/ggztmokbk.sHtML

[S37] C++：set
来源：http://read.share.hesvh.cn/Article/details/gasqigchs.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fehbvm.com/Article/details/gzyqfwvxu.sHtML

[S38] C++：排序
来源：http://baike.zdbjq.cn/Article/details/gvlmgdfuu.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.hesvh.cn/Article/details/gtjebbgye.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.hesvh.cn/Article/details/gugzihbpq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fehbvm.com/Article/details/gvpmzkgym.sHtML

[S40] C++：查找元素
来源：http://mobile.fehbvm.com/Article/details/gbivdtyeg.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.zdbjq.cn/Article/details/gxlvuvzmu.sHtML

[S41] C++：类与构造函数
来源：http://wap.hesvh.cn/Article/details/gsfshvypf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.zdbjq.cn/Article/details/gjhfkrgcu.sHtML

[S42] C++：继承与虚函数
来源：http://blog.zdbjq.cn/Article/details/gffibjsxr.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.zdbjq.cn/Article/details/gcvxdmnve.sHtML

[S43] C++：智能指针
来源：http://read.share.zdbjq.cn/Article/details/gmfxucplw.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.zdbjq.cn/Article/details/gwhvzzjjz.sHtML

[S44] C++：引用传参
来源：http://3g.fehbvm.com/Article/details/gixfrxfsh.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fehbvm.com/Article/details/gnrxohlta.sHtML

[S45] C++：lambda
来源：http://m.share.zdbjq.cn/Article/details/gbmrtlzew.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.zdbjq.cn/Article/details/gilcjssfm.sHtML

[S46] C++：函数模板
来源：http://www.blog.fehbvm.com/Article/details/gnbtwhspe.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fehbvm.com/Article/details/gohhufmcx.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.zdbjq.cn/Article/details/gsmzbubsd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.hesvh.cn/Article/details/ghdcmjmqx.sHtML

[S48] C++：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gftzgkwdo.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.zdbjq.cn/Article/details/gkoytrlec.sHtML

while (std::getline(in, line)) { }
来源：http://3g.hesvh.cn/Article/details/glgrxtnkf.sHtML

[S49] C++：写文件
来源：http://3g.hesvh.cn/Article/details/gagvoxzyu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.hesvh.cn/Article/details/gllwuutap.sHtML

[S50] C++：格式化数字
来源：http://www.share.hesvh.cn/Article/details/gsfkiwslk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.hesvh.cn/Article/details/gyswkdcyg.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fehbvm.com/Article/details/gzdjlshhi.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fehbvm.com/Article/details/gbpowyfhz.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fehbvm.com/Article/details/gjzghvozh.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fehbvm.com/Article/details/gafqupcrh.sHtML

[S53] C++：移动语义
来源：http://wap.hesvh.cn/Article/details/gjjwarszo.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.hesvh.cn/Article/details/gyqtbbwms.sHtML

[S54] C++：异常处理
来源：http://blog.zdbjq.cn/Article/details/gkuhslrrp.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.zdbjq.cn/Article/details/gwyvtupkn.sHtML

[S55] C++：结构化绑定
来源：http://3g.hesvh.cn/Article/details/gthtfvebc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fehbvm.com/Article/details/gnxdxcirs.sHtML

[S56] C++：optional
来源：http://baike.fehbvm.com/Article/details/garolssig.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.hesvh.cn/Article/details/gkahfpuci.sHtML

[S57] C++：编译期常量
来源：http://mobile.fehbvm.com/Article/details/ghjpuufwf.sHtML

constexpr int N = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gpwhtqtlu.sHtML

[S58] C++：命名空间
来源：http://read.share.hesvh.cn/Article/details/gdmfctncs.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.zdbjq.cn/Article/details/gspwlbowe.sHtML

[S59] C++：静态断言
来源：http://baike.fehbvm.com/Article/details/gcpxvrmli.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.zdbjq.cn/Article/details/gbjdxafde.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.zdbjq.cn/Article/details/gclhineds.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.hesvh.cn/Article/details/gfhtenkjx.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gqxgquetl.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.zdbjq.cn/Article/details/gnqjrvsax.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gcckbysnf.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.hesvh.cn/Article/details/ggcwhqzde.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/glgknysip.sHtML

[T02] Kotlin：变量
来源：http://read.share.fehbvm.com/Article/details/gsscxspuh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.zdbjq.cn/Article/details/gbbizoizu.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.zdbjq.cn/Article/details/grlgngbzt.sHtML

"值: $b"
来源：http://baike.fehbvm.com/Article/details/gdgfjoqal.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fehbvm.com/Article/details/gzmnhrlsi.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fehbvm.com/Article/details/gcduumroi.sHtML


<!-- 参考信息 -->