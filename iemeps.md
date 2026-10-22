代发 wailian999

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2msblrlhz.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2fozplpdb.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2guachuqz.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2muuxjwni.html

esac
来源：http://www.52xcode.cn/Article/details/gt2fqimjxms.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2dobvwqrd.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2dxyxivbj.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2sxslqrns.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2wwhdzing.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2qynvtffa.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2lcfcayws.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ssnpnvoi.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2svenrwgg.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2cpcscvdr.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2zyzyroui.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2ypnrexww.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2xqczaoxb.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2hgcgdwan.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2hfbrhtmk.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2vbpsmbxa.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ocxowpdg.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2oojhwgdi.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2jxnqvsyu.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2lsjyyfuq.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2yifapehd.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2iqiqrbul.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2rqxyjhku.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2jebiwkdp.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2lbllrqah.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2tfoizzmm.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2bjksdrun.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2lxpkcfvb.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2uqbhulqz.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2apbdhlxz.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2dheffuig.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2obrsebsb.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2nvgqixcf.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2rytbtzpc.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2wwpvhanv.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2gfoymilq.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2kjjscfak.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2figuolur.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2rmulrnka.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2rcjiwsvl.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rpzbrxsg.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2pugdgxfx.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2zibdjour.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2xrhyrpzp.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2ohrusnvl.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2pbtatyer.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2ednixisi.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2qrjzyrno.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2gbtimwxb.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2bdcnmtxm.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2eoporzab.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2ctdqllbc.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2urtxxppt.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2pppzudrp.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2sbwtwmjv.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2ewsbdwud.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2qwqrhcha.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2pcwgxovu.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2fxauxnax.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2rfdfzivi.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2kvctxtfj.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2bomeaqzu.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bnecqbgz.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2rrhlrtye.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ejpsarol.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2kyljqaqy.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2sfjbrufl.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2bxkosnpb.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2dzbsatsy.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2kowojsjh.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2iheviyvn.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2rhpffngu.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ihnkbkwd.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2urhragbz.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2wjaojrym.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2ukchaleo.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2saskfwsp.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2stlrptxo.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2uxesyncw.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2awljhsrj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2azjodptu.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2vsswqemh.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2lmudzeiz.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2lgqubxfl.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2vhblmcdf.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2hhplgafk.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2xjunohmo.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2exbzmhvh.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2rmbsrynq.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2vuyqwxll.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2tezfaauj.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2nreowdnf.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2jxlttces.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2tjkxcupo.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2nspmsxfn.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2gyrjjcmz.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2oqbvrjeo.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2cmoahqkr.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2fzfctksf.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2pcpfwrnf.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2hquejeig.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2bcwfxgdz.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2dxnpjmaj.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2uwlbstam.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2gcfvzaay.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2efdiewfw.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2wbhawoqc.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2fupctnkd.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2zlpshewv.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2skwqpkny.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2ppgfkktz.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2zpfefgap.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2gpdipyfq.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2srldaaww.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zeyvjkwf.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2qfdugikv.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2fmxmumaq.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2smdokobs.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2kbvmiidu.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2jxiqhcjo.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2ohaxdxff.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2xaaldtni.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2ylutawqy.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2dgvtnruh.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2sjpmfkwj.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2cukirjdl.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2hackvmeu.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2ffwdfegn.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2xtpdltbm.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2wqwtapkl.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2icgijsdi.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2jbwfvckt.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2zljeofcd.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2duoacemo.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2eihackay.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2uoomgazi.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2sriuxikh.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2wdcjirra.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2ujruemps.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wwptamrs.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2nkghhtrf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wdvyxwlg.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ypgmxloc.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2qjyetewz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2xeutdjdp.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2hrfpmkgi.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2fhhfaaip.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2fwxmvome.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2dvbnashq.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2vtayhkxl.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2rblrualw.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2qqfgmoxt.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2ebbiihzf.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2jffjheak.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2eodgxoov.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2yomzhkfy.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2tkbleobv.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2loaporta.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2mhdqckqu.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2qcfigasg.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2ilfxbjyq.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2exkrrijn.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2ltbnrnfq.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2vtjbtrjx.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2xwmgfxdz.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ofwxfdyc.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2leltsmxb.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2mnoepwcf.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2yebyufnz.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2mxmwfexq.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2avbphkyo.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2ednfkhzt.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2cvyqostj.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2irvtksyf.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2pagbbrzf.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2pwsuidvs.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2kqdpigji.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yalqlowy.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2stnrseya.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2yguxyaua.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2ivadpqgb.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2nquuudpk.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2osrubmjl.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2fbznoihl.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2lqpzpqfh.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2vwrvqzsv.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2guhixmzj.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2icuhdcab.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2mxvsrazn.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2qfpfplmf.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2jwpurubh.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2lzpfsihn.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2ueobepyu.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2amzmrspt.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2pwtuhkok.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2dwvepjru.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2gkhpgorf.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2pzfozzfd.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2mutmfhox.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2cgnumiuh.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2nrgkbjbs.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2lzxkhceo.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2gbdvtvtf.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2qenkdoed.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2bemsinud.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2bxylfdti.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2dltpkucy.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mvqxzhon.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2zvteztyb.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sofnmcvb.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2cgvafzcj.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2qeochmrj.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2roxwxntd.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2bqifgjlr.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2llyvmkxp.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2eliewlch.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2cpsextyz.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2vpfycyxy.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2zbztkpov.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2elstqwul.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2nhnpuypt.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2mjrnptkz.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2luaepumj.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2wjsptbpg.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2crnpxddn.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2fejerwel.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2krxwolmr.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2niedehxj.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2azatkvfz.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2yxmsirop.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2nkrtuhgi.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2dryhtwpe.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2swagicmg.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2hwvsxhrd.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2cvicdrpp.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ivhqvzel.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2txliynml.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2tzrduuio.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2ohvupzdv.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2qldjsorw.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2ljocehkw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2qnjspgmi.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2gdrwswba.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2uupawntz.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2uhexvcdv.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2urneldhz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2aebehqcx.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2upzmgdkh.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2usobhztj.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2vwhgjtpq.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2cvmjurub.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2iaksqbzg.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2oondkhkz.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2jllrwzrh.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2poacmzho.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2vdvwjcon.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2umxwesmx.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2wszrcfyx.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2obcfoaem.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2vouzsdma.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2ywubqptk.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2ifmnsvpg.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2uhsbpwnu.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2bymboaka.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2tblxjoag.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2prvzsgwo.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2ffnbkmvl.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2mmiykjrw.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2llsmczke.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kgyboozb.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2zjnrozty.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mrmhhdys.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2rzvvbdvg.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2vsgkqelp.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2pwcokocs.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2tpdhvyuq.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2djbqdgcd.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2ltcwpxga.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2hroocuxq.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2wjjtexrj.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2nsfgyjxh.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2xjmtpcvx.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2zthleacl.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2zghxtijb.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2imckyplo.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2verqhrzm.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2mbzvedbp.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2wpbawgyy.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2qkdgjrxd.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2lopjcqzc.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2awarfizd.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2zpdvygxm.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2jfetedno.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2ryoaphea.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2jxirnsgg.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2arhzarzr.html


<!-- 参考信息 -->