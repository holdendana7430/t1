代发 wailian999

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2tplxwnfe.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2fsbhxusu.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ekixpniz.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2bdjgagno.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2ydvwgwny.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2vziblavs.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2hxdfdvum.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2lhvscedq.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2mbjluqtg.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2qjidhcns.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2mpfkuwbn.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2eqrgnrvo.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2siuhidqs.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2jlxrwcjy.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2vlbnmtme.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2dqkmrrde.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2ngchihcc.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2rkrkwhgt.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2mlzjzzhq.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2hdvotivx.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2gpxzoyti.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2duqxlqvb.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2tzcdwust.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2bqckahaw.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2bmpphqdn.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2plimydgp.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2auhndxnf.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2ppypdhvf.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2hbwonegt.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2xqtgakvm.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2qkyfmram.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2jgkdayvi.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2qoqgopvy.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2phnmvrbj.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2unlipkrk.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2fejmdrkd.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2trimucdc.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2sscghhet.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2pxelzgvu.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2xdewhhjg.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2vaxlbvii.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2cgolewxy.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2vevdjhov.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2tcqvoeol.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2iovnhkgl.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2tiinfblr.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2yfzfoikw.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2lubwpkvz.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2bmcyjcvu.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2agrdmhbh.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ejcjefwu.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2alnietrj.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2lrpxodno.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2ucjkmpmp.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2aachqenl.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2mowgpwsq.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2lgeosvxg.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2xkkwjqem.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2nuxwgoes.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2cpwznbhl.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2ranytkqb.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2vfwyzwiy.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mfjuwqua.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2ezgehlga.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2ubeittff.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2ikgxdyyx.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2oajwlexd.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2irkiwadf.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2okerzqqg.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2msbsrmwn.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2yyrlpcwn.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2kiazptnv.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2sfuywalq.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2rvlvkfbl.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2tjtjhjoq.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2tqzosgpb.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2uxofzmsy.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2uxrtrywd.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2narxqpdq.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2qlvmcyhe.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2vjlygylu.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2xcfbxfjk.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2vexotrvo.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2vlptsmok.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2sovglyjb.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2ivdexido.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2ewudxzmp.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2efdlltjy.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2kqfyyiyl.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2ifkylrxt.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2tybssvio.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2dwbvpqtl.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2zykbeple.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2xopcqehf.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2sjolteyp.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2gjjubjdo.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2tplpxfjq.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2cpkbqtvp.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2ctryamhq.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2cmcgnawn.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2fkzvyjby.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2rjxzpzhd.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2pipwvhul.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2nbnvwqgm.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2kdiaxclp.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2rlsedawl.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2ohbsdsor.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2rgvdtopw.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2dvjapllu.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2vjrfyxzy.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2kwzmqjau.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2yoboicoi.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2qqylttwm.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2goeggpyc.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2kfqdvycj.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2ctzsnoxe.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2bokbfkya.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2abgximon.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2mjkficlk.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2qscsqlsg.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2mlufqnsy.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2nixsluag.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2hmffhkdd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tezvllpa.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2ctajazol.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2koyteaqo.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2cjfcpzyf.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2lypergsv.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2xbdvpuks.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2tcxmhddk.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2ljyawqag.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2oucchget.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2xxdukczu.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2ozfdyqca.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2typjsvyx.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2syxsbdol.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nwjithmh.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2xclkutgu.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2helqwxlg.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2dqwqtpvi.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2tsndrtiv.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2hbcgievj.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2saqdptxw.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2redmpckk.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2afmtqxsf.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2ufgvxsoo.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2btivkqco.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2djauwcxl.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2xmjepavp.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2sofvklzm.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2jzngttqx.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2uwpytuos.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2trtrftrb.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2ejjxjrtu.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2xedqikhp.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2mvasqhaw.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2jjyfclzj.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2tyquhorj.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2enncjuld.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2espsofka.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pkaviprz.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2tllxxoxn.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2yvlsygwc.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2ahmgjrfs.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2mroxaxhs.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2npdrvklc.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2qlkoihmy.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2izgvanqf.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2xquqbtgv.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2uecybiix.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2dmyqlhzp.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2ymjvcern.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2bahtkrvc.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2kylmbpxg.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2cvbjtlnr.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2bvncnruk.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2jhbwjfju.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2odxeijad.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2jqayokri.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2edgetkof.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2bosbyryc.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2bofbbaxe.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2qqwettbp.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2bckqmmlv.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2jeetjoge.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2vpjmpwod.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2oohnggmt.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2jqcuodgg.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2eumipjiv.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2ehvoemlz.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2bkyjeoul.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jkfruber.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2mmtedifs.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2rhlfvigj.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2axbhnqde.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2tddlxqcf.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2fmktjcff.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2njghpprq.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2sicusyoa.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2twjpukiz.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2rtcatswr.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2lhjigyrs.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2eqfbopav.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2binscwva.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2lwndujju.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2cgkpiksf.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2jdpckwlq.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2jshsepvo.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2uflfhzol.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2czrfwytb.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2uiehofvd.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2gvswrzjz.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2sfdxnxvw.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2mpegqqux.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2fqnmxmek.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2ddttldhh.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2bbvnjxie.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2yyypsqul.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2sqgzibuo.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2xzksrimy.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2pnoyirox.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2xufajbsh.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2kmmvuigv.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2rihgmslj.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2tbnuxfcj.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2soerccgd.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2dysfgsbn.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2vifedxgb.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2wyiumbac.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2uwibtcva.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2ygcwbyiy.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2wfhacdib.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2mkngeapm.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2ipghwchm.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2mvxrjxpw.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2ajevbtbz.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2jlwkcefa.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2joxqgflq.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2awmribnk.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2yitwlcfj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2urczrolk.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2epzncfvz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2sbkmslor.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2ndptqvvw.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2gmruvbos.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2vqonxvru.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2vjzwtrym.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2qjwdwkgt.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2sbxixdim.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2sbpcfvir.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2hujsfyux.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2sllphkac.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2gmbbpkko.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hgpzhtat.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2gvnikjln.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2heqbiyqk.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ezobwyno.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2yktthnat.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2rxjjquhm.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2xvljqjgd.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2myuuefbk.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2btahvqdw.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2ixlozqtb.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2wqjkrlny.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2lddnsiwf.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2ubuvyzkt.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2glkmpund.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2fcfpxjzq.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2wddudvnd.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2gytzyxhf.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2jmjktdih.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2jsxhwqnk.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2jgzbzeuq.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2fmnnernc.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2hdieniyt.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2tnhibmds.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2qzqpokks.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2ymsxjpzt.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2pfookiod.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tbyeoyto.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2sebsdcsf.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2xpbsnmct.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2bklqqzjw.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2vigtcfmn.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2vqkmmopk.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2mejgcllq.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2dnjwuveo.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2lswemsug.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2prpbbyum.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ulabgcvu.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2grtsabcz.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2dwqyfsuh.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2grpoksop.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2swowigyw.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2noyafxmr.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2lhduzurw.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2uocymopc.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2zqhbruvd.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2mpgvuktc.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2xmmzdspl.html


<!-- 参考信息 -->