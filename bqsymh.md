代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2nutwfrnl.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2uszcpxza.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2xkeobeft.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2vcivtltn.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2tocupqdp.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2tylvcyyc.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2avzvmglu.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2xxyologw.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2ydrfkoxl.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2qckurngz.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2zlhwzutt.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2mhvfcvoc.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2tpgfmack.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2kjjdmotq.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2xsmgolby.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2nqkshyxz.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2whdwdxgp.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2gpshjqvd.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2gdqmhhhc.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2jalrmvxp.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2chvejgha.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2snnqijxo.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2tbtrwbdw.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2zalvromg.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2vnpsnngx.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2axvnxnxh.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2dehwiksh.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2xbmjwmlf.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gnwlthdr.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2jwvcxois.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2irtdajgb.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2qjxnsxqp.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2ncoqklkb.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2lbjkqtdg.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2plmasbae.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2jiwcfyba.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2gftxakbk.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2igftucyg.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2wlsmbaqr.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2cqwvbpfr.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2fhsmpvcq.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2epirntyp.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2axcqufnu.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2dwakhner.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2jlikueuc.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2fgnlqwbz.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2wufjmcaj.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2bjlxxsoa.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2qckmjrqf.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2kxvpllxq.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2sszerhsi.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2ldyngjaj.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2kazhmjjz.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2ktquiogq.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2fghpzyuw.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2ookpluxf.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2bfxdsvnk.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2gapvyeox.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2uybhsjux.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2iklcylmk.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2lbypkfyk.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2devudpnr.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vduyuoom.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2jmnovamj.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2opbqsdcs.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2lgzxzjwl.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2lzrkhueo.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2glakihpf.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2jklbczuu.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2xyikgsyo.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2twjsdnaa.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2wncxyaci.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2fkmagpio.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ovrerwmk.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gqgmmrdb.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2lgqcvvae.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2uqneahxk.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2oagwitbg.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2ofoabyry.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2hrhndkws.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2izxdmsde.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2zlhianvb.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2flilkmxb.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2finofgqh.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2geugiodw.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ilyialyr.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2usjalbyi.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2xkypgsij.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2gzrlycyg.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2zbgldizu.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2amgshjgy.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2vndiblgq.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2qgcrylij.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2dakhgevr.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2hcgcizqz.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2mkabouzv.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2waollvnl.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2gqkyyyoi.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2zqdtewsh.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2ufbobdue.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2mlrlkouw.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2lpwhgllo.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ntoywzdo.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2gcbymhiv.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2ofphhjgt.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2qzupshld.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2ymotrqix.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2nlulupds.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2sttyhaci.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2uohtnluh.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2rhfqiipm.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2ytukjfcg.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2rntoivzw.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2ssygsdml.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2cnoosdzj.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2ywfrpxsz.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2xzszposl.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2xtbbsbcs.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2fdfybelx.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2nzjjqnyi.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2igqcdqdk.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2qbwpfwhl.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2fwiurdxo.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2muaxumgh.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2izevxpwk.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2loewyhbo.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2xtuymccs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dpfhsspf.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2tpzmxdcs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fheujqhk.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ihqtqzqy.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2dgwjuqqd.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2zcvazagj.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2motnhgxu.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2esmdllco.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2thrawkxp.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2hjnqvtci.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2nidagsdv.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2puyftszj.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2tshlzacf.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2xfnpwqhv.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ffguapcm.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2xcuictsz.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2yzyqiqbt.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2tlruvtqa.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2xpxxbgut.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2nrmbsnba.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2vvqruyfy.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2butenvmm.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2lqgvyung.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2ruhdzlhs.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2dbecmwxg.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2beorwqdz.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2tjlskmyy.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2nnpoxrem.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2knxsyege.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2kbfdeldp.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2xpztllqk.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2guxewrkn.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2lsewwotx.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2mxydzzez.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2wnobprrr.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2cywqhstb.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2omhrawnl.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xemddyxc.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2huvmtswt.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2bnfiockg.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2nhjlcwfj.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2vgojktwr.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2gkzzeiex.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2aujfjrtd.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2ghuofxfn.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2dllqbydf.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2mpdibomm.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2oeqqfqdg.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2cwjyqemz.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2qwltltpj.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2luaovfqy.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2tvqjeyzn.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2wsqefniq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2blainexb.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2udjugnfh.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2flirnqkm.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2nbluegrc.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2tdbhbcuy.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2ppjswpxm.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2svdeqzyp.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2ykonqxga.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2ktvjupxg.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2ynihvhrb.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2rafeycmr.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2rcyiohid.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2kowwkoec.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2zwwfrsyk.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2hbbretrh.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2aooyfzbp.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2sdbbekfm.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lqhciebu.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xbqobhns.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2fjuhqovs.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2lyepgfjr.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2rwyickxw.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2xtlxrmys.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2bosqzgqt.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2tdandpsw.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ttvsfknf.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2bamxavlk.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2kewlyndl.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2pjdapxfn.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2vprbmujw.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2zprsztuq.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2lkgmpgkb.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2jfnzxium.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2nropsgug.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2mtobyjdl.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2xtseqgbm.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2wfqjtvxy.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2kyqihkqw.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2swhryosd.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2jphmzfav.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2uqwhlabl.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2rvegcjpd.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2qbjhslud.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2ykknduhp.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2gglyybel.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2soivcchg.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2ogzbzfmu.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fdwyscct.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2cipmczau.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2ucnwwcvq.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2dbpqebrp.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2txffgkht.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2mrscgjpq.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2uiicexyr.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2luflxbrh.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2alochimz.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2znpjdctc.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2hclkstsi.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2fcebeixh.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2adlwispu.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2qgnjvvig.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2frrtqllw.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2xgqminxa.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2yxyufipr.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2nzjtqfri.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2zjznuosk.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mswcfyuw.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2rrpzakud.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2bznurybo.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2zjdryhgt.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2hyzxrsil.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2nhcwumyk.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2qyycgntx.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2pxprcmsg.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2yvwvkwmv.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2qhxgcedx.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2xnkeeyvv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fnqpiulv.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2uitkkgcm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ziqnqapc.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wavukoat.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2labojyko.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2gtscvdtp.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2brvdnupi.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2wnyxddya.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2uliqpwrp.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2lbpjtmei.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2nnaogvmt.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2oejpempj.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2ufdaqpli.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2hdpsrmkq.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2gpsvmhib.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2xcfvbyiv.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2uiwrikbv.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2yttthltr.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2mzbmywbw.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2upsxxokg.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2zgmbplll.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2syhqaszt.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2obxrdmqd.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2qoyxidvx.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2hbllycfo.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2ghxqthmj.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2klwgpffd.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2sfkabuza.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2syjjptid.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2bhxieqob.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2hjmdgdkm.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2dftfvpam.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2vtfypbdt.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2prwrrfcz.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ssqyoflh.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2smrreonv.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2tfvqosbt.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2tqkvvdcj.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2nrmciwao.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2qvjfqxew.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2tvvslcrh.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2latusiya.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2jsimlozf.html


<!-- 参考信息 -->