代发 wailian999

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3krefijgj.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3mrtxihmi.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ndnwpqfb.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3bejgjfum.html

esac
来源：http://www.52xcode.cn/Article/details/gt3httypykj.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3dkwnlcng.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3aeyqblwv.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3uxprvdvp.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3hfafmwnl.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3tqlwtloi.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3faypapeb.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3jywxlmnx.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3aubyviob.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3ggmcnxoo.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3oivcqvgc.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3rvuynxec.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3dxydgnar.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3hgqjtjbh.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3cdttzqcb.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3jmoltffk.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3qnkfyxyq.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3bqxqdncv.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3rpeafmkk.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3gquoecmv.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3astwwyfc.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3mlpuzpqt.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3gixlrwls.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3jwhthlqe.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3tdqtzaoe.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3fdgjvuaw.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3yfdggxdv.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3frevjerw.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3dwbdedof.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3memkzmvw.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3mxujaupn.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3zjcupdzb.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3knlceivc.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3oxgdvkkg.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3qfqruicj.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3fuzljcpr.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3zfpvenlm.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ynjehhva.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3gjwkaxvh.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3ykdbfmdo.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3arsotxfl.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3fttfcjnf.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3jeungxst.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3ubioflao.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3gvzihgyo.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3rdlaltte.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3nthjksbt.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3dogggncw.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3eigupfns.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3akpnxbpu.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3orveiycq.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3hbdwcsvq.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3pnoatvbg.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3nrdizpup.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3cbyhuzjw.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3nqdolprv.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3pbwzkrbw.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3ukyuqdzm.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3xunigjjk.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3xrvlqtbb.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3jnnmtbkk.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3pyqltukb.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zrcdrowc.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3bzuiuziw.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3qubiexil.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3gmzrtqpv.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3hdvbbpls.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3tkytawno.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3sjljxywf.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3fypjyilh.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3aprnjudt.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3msvpfjxz.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3wdiadchb.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3aotbgbnf.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3yszvfyqk.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3ehrkrabl.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3vuxoekqi.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3wgocisme.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3bocutnop.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3cxwlighh.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3jynwqxwl.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3jfwgueqh.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3ftszvtse.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3ljqgbqvm.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3tlzbequw.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3kikoaoly.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ktrpjzfq.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3nnojucnr.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3leivbtdq.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3jdcicaly.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3ydqrdnvy.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3lflatrvy.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3twkwtour.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3uxgjijxj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3dpeckwjd.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3czyefhnk.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3qzlsellu.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3wwsgebrn.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3gbzqkvmt.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3ajdtrvns.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3dewabipe.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3itucnjca.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3zvftmhca.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3yyheirvh.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3cmzlmbmu.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3kisikzkt.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3gnzwnzgd.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3msgaepwp.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3cyeovicv.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3pojkyayt.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3komkfvqd.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3erbajxfs.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3teuynnpa.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3szumidbp.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3naudntpb.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3ahpzwzsd.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3viceqinc.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3oyrrwnsv.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3mamqxgut.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3owvdtynl.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3mqeiaerc.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3ebnnkuyk.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3pgwwdxof.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3pexexxpu.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3asahhfhg.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3bnnncfak.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3dllnmrwo.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3yspivger.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3vyirjtnu.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3iyzxykts.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3hyjsxbtg.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3tsfgjhgb.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3vlnrdadg.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3fsjdmlpr.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3vjulmrqt.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3hbuxoriy.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3hixsgypd.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3fvdsowuo.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3ybqixnhr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pxgmjnzh.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3yuonxigh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kigdsjbk.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3rzzrvofr.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3txasjmpq.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3btqqcnbq.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3jrzztoub.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3mvlwurvj.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3xwvssnop.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3akpmzdbf.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3xhfaixxu.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3xivqfhum.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3kioybmbf.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3beavhzgl.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3cljothsd.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3cnlvsxbt.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3limnoetw.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3lxoztqgq.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3dkiirtxf.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3hfbfbkfo.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3dwdddmrv.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3wtcisqww.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3fyjorgkf.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3awxmcvms.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ihvndvbe.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3gqwpysxk.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3cwbcoirp.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3qqcehvlq.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3ivzyxtml.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ejyusrva.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3rcwmkvdy.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3nmyaazof.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3uxuwvgrx.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3swgnpajk.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3qbyhuqvr.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3nurtxago.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3tvoewriu.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mdjlygtl.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3fduhkzjp.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3yzvcuina.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3fvhthhic.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3nkoxgebo.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3solcwfpc.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3csrxfcri.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3znudttve.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3hzrfkrwr.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3dxlgkgtr.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3oemzmaui.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3mahsrxly.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3ovufognn.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3kmvcpbcv.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3kcxbrqxd.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3gvuktgwz.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3gjbagemx.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3plkyuxfq.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3zueldiyw.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3jlsrwcjv.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3mtxoquap.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3vyqyiorx.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3bevmjklb.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3bfmdkutd.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3wjgnmnhr.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3zwxantyb.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3afqgjqsm.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3hrqniesc.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3omsfjgae.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3cdzvifbo.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3tchyespp.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wcmnsjav.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3bpkpmaxk.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3nytevlno.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3rwazspqp.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3rcjvxddk.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3lugwszsd.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3rjjefkkc.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3gkacpqjm.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ocpwdchu.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3ymehrzos.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3irlleowz.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3kcccdqeu.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ihpnvphz.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3fehcnwna.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3cdcmknkq.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3dnxrsmrq.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3bhswqqpl.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3raavgsah.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3cdqfqpkw.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3ogerthqs.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3uypdoejp.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3bqnyrurr.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3tkknicfc.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3lnxcbrda.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3fwzfyrdo.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3afkcgppx.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3sbcvdwet.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3beqyxihw.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3nvctmljm.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3yycpcwun.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3nsxwjjub.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3dbviwzun.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rhlexcsj.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lpkjkmog.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3wmpymmmx.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3lzruuxul.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3ymnfugzg.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3lumdlwma.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3edmdpupo.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3crfwxpxp.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3dbdyztbk.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3gqmdhkut.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3ludmveup.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3lvdjopue.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3edmhgimt.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3izwpuafl.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3hgyjvoln.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3nujrkvnw.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3jovzdupy.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3wdyunuqy.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3zfxazlnu.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zkpatpfe.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3pzhkrozb.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3uwaohown.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3qjuryxbh.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3rrpcuxma.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3hsgrtmmu.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3atlmwtyk.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3umsvqeza.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3yuwhjadf.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3ajnwimep.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3uqmhzenu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nnwtkoiw.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3ohyefuff.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nahbmqft.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ygskrbwk.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3cjsvgqmz.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3dkezigst.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3zsedbbiv.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3apmuslrx.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3nmcuanvl.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3kguhclpi.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3gyyubvwi.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3czacucev.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3ksjdmzgc.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3msifvzwa.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3qbkjrrqs.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3cibvests.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3cttadlmv.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3ochecugc.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3qoepmqvc.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3dbwqjczj.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3haxaixzy.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3abqrldwl.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3ldqzbker.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3onpnswee.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3uhklzazo.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3ytelyadh.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lfmxpvis.html


<!-- 参考信息 -->