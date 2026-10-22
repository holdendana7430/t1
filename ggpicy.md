代发 wailian999

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2owxnenad.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2tapvpcuh.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2qaqlylad.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2sknzlmhh.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2jsgccdkx.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2offdsgyw.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2xiejkwum.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2jjsgbdml.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2yvelkaxm.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2gjipdpcy.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2jfwovpll.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2qvciblin.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2wcagxjca.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2gwlhveij.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2mhgydtxe.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2ntxriegr.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2jkboyilm.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ikpjmbhc.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2cxuinvsl.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2uqkkzmmu.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2rpyhxpwe.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2yobubiza.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2syadhtij.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2sdtdshyd.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2wdstavfn.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2lebaanbd.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2yghimuxg.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2zkjnnwde.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2otkdambc.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2stpmvuar.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2hbkdusrt.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2tumrxhpr.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2mmxemhyc.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2lllewdpl.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2tqsvycyh.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2qsycdktk.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2dwsadlsm.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2fnxgktgp.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2tkxqbaaf.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2gwsltunj.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2ezhporbr.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2kfmcwhdw.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2knvkxzpr.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2wsrjwaca.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2ciffsbyp.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ykwynejn.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2ejscuiae.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2abkygehv.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2jayrbyex.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2cfgvfjwo.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2kvklmcbv.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2vwldlmkg.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2rqtuumxf.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2vnvvfdmt.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2wtehzpho.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2esnxsxym.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2vtgorsli.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ijdbkmiv.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2axamlbam.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2mqfqaaav.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2oklfaafq.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2hjacytqc.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2xloirfrb.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2yawwrrqa.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2wzvrmjab.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2mrucqymn.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2csoklktx.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2gmqhtoth.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2lgljltuv.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2mkepeekn.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2xsueuzju.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2ovemafpv.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2wggnsnty.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2axruikko.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2mkrzzquy.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2vxkhycoy.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2wnsqqpmb.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2dqvblqdj.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2lrilupgb.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2itjzvvya.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2yfnyfksj.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2lpkkxrne.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2zeiacpoy.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2mhkjnawt.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2wrejmyos.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2rkbbplzt.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2mzdbycae.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2akrcbqnw.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2gyzvxaui.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2kntqzjbx.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2ecjbnjta.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2yzkkhwdf.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2vowcauwj.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2ffczjyif.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2uxjndokc.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2nearrewj.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2bfaxfjpp.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2iqsfqagx.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2cvghubgv.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2yoqxvggq.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2prafpgal.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2uxomjjnx.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2qmonucyw.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2zwoxwnhq.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2geoqfvha.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2rygtoyzf.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2lulyvgks.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2tbfyrtul.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2ydogywsh.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2legkjfkq.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2efsmfphf.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2cbwlpqrc.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2ignanvvs.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2wevqolks.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2vtghnlrg.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2cgdtpelc.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2ldxvofdz.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2jmqkoorp.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2rzfcdkxn.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2veabhhyj.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2piadthpp.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2bulwtvss.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2aliuasyv.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2mqtvchbv.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2glqlvjgb.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2fsqpmfjd.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2aunbriiq.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2gpipbtqt.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2jmxvedhv.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2igzlvnyo.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2qwekrtmi.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2mlgwwuzh.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2yzgutfey.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2dpzgrjru.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2gjkrqtig.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2vuezqgsz.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2fekhxcdp.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2babcsgub.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2mifhmyxi.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2nxbgtxcl.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2ciifczqs.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2kjwrqekf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2jbcituni.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2yooliklr.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2dzfcqzvp.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2urenlnhb.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2byaetuvr.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2apxwazni.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2zqpcugbr.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2ywgceqbs.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2jolsogrk.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2rxsuthrx.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2ytdureug.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2sbxqzyaq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2alaoilkd.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2jcvgqjgc.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2ulwpbjyg.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2duywpnwu.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2qmwkapzm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bqhkzekw.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2jwwuleev.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rnvwiwje.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2yazaznfc.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2htlammbw.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2agkvgjtd.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2kkqcpcfh.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2prvsdxap.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2rwieqxro.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2hzmhhqon.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2ombwvrmp.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2hghdqnze.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ssplmggm.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2oednelzt.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2bugyypzz.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2ppfyfbch.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2rtbvoxgc.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2yweqkvsk.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2orielxcy.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2ssvokbvm.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2wldsyvij.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2rocdizqx.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2idrjvedi.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2gadgaofx.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2rcejyztm.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2ahppnijx.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2cgfyuksq.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2dmupjfyj.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2moqxtkkr.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2obpbsdyo.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2iziegvls.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2vxgaztab.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ymzdkhxp.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2nlpsulav.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2njepgpmd.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2mcdmgles.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2brhzandv.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2dhawxeqb.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fvsyezvr.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2xuzaluki.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2tthlaqvl.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2dxfrgfxy.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2svqswjyd.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2olwsarpf.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2ywhgrrio.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2kwkeljar.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2bdbgriom.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2vebrfmsg.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2tfgggiui.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2nyxmadit.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2pbvdrlck.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2xcgyhyus.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2dwrethev.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2vtkylhks.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2ciswfkfb.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2hbjmyhvk.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2hpvicbjr.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2wncfiusm.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2ndqrvyec.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2oxxhtotw.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2mtogvdqv.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2ufjsojuo.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2dqcihumn.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2iebomykq.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2nbcdnmhv.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2riocbwho.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2xzekvgsv.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2wdjthxvq.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2miqefqon.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2cscqnyoe.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2pltgktut.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2jrchibij.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2jmmuwexg.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2unguusms.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2igeoiblf.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2pjtnmhuy.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2gsrdqfgx.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2fhgxqmvk.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mursvppg.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2yqnnfjrz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2iqezbevn.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2koabjisi.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2prrkrdat.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2hlkrkeac.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2aiztfnhg.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2lewplcde.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2nlgxauba.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2xruirnjj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2bftdftuq.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2fqqwowoh.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2oemnjmls.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2mrndlegi.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2jjwejnvv.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2sdospqnc.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2mruylloh.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2zlklhwbq.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ktpfwayb.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2cgwwwbjv.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2gevacgbz.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2xbrgducx.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bkyzqhip.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2krrxmega.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2thbqkuxf.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2clmmozve.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2fdcppijt.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2hjskiewv.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2tmqvxghn.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2dowqztmn.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2dlzreaql.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2zfshtpsy.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2iqmlfvun.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2kxrxgycz.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2cqtvpxxf.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2rbodpvjh.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2euqhmkbo.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2hgkhffme.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2rxrlwgmu.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2gvvhrhky.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2yfsxyghx.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gdxqugyp.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2uflebovx.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2ubpebncq.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2dfgycndo.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2tjmrtbcj.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2drrfthkp.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2jrtmftvp.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2vzdnnkpd.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2metubnrs.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2muhjdspd.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2hthywyim.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2umrnxkuf.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2styumiao.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pznbwyud.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2uoffpkxg.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2shzgrthm.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2frnplxjl.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2immvkygi.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2lsotirmu.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2jnruscsp.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2cwggzira.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2dmrftkdj.html


<!-- 参考信息 -->