代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2clqcgmeo.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2lzbozhdg.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2rhkyyadp.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2bicovwzl.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2spykgept.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2ojsifvln.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2blcwxzmp.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2blzyxuby.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2rkyoofzq.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2lwxndndl.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2pulruquz.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2iorkshed.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2ttdxjkmg.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2umiaxpjs.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2raauvfik.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2maxmhysh.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2zvvmnmam.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2kvygjwqc.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2kpdetlut.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2nntytynf.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2djknuvlc.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2xeedzwxd.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2ygzjbiwq.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2mbqbungo.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2jiidecej.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2fwwrqadv.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2wasdebdf.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2fqldfnvn.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2bediqjea.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2jbuxkpga.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2nikpicyn.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2xemussoj.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2tqazjzef.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2szczncxb.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2hijqvrjj.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2fdibtfre.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2bqkdebyy.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2tvlgmymo.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tzxeiqqz.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2hfhjorpd.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2hilxqfha.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2sckoojde.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2gmzstvim.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2egkqxxrm.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2rgnewkde.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2aeooohvo.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2usxuqkht.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2iyyrxxmi.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ykyymzjg.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2dkketdrt.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kzfdhiom.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2kwkvqpgu.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2ruxmxamr.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2vhqggszi.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ysyzdefo.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2ytjqrgig.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2mnjrtehj.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2esvtvmjo.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2guuanoar.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2cecugixo.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2bapwflvg.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2gsyljygn.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dmmosnsm.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2hzmcimtm.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2bnskudqa.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2afbnnvmt.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2uncapgbg.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2sfddbrrc.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2hjhlatbq.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2crozxrsp.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2amqehaca.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2deyrifdd.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2uyihmham.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ekuhqpnj.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2qetubypo.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2doaivyws.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2qppzvehz.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2thtbofas.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2wvaagsri.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2jktwpowv.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2epiaoafp.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2njxdcnpi.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2zlsbrefw.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2oelyzqal.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2zwbrfujs.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2mqcunckt.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2wnnbvlhz.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2xcfrkple.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2kftxwtcl.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2hflililc.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zrkgbmoc.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2iefmrpfw.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2gdtzhdte.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2kfmmnxeq.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2sinwogsy.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ujmukwfi.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2xobhjfzh.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2lmknpmwf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2gqxetqwh.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2blqpdsca.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2ylilpxlr.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2nvqcjktw.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2csnsdetw.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2iqmpcarw.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2imuixrsi.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2bzzoewvg.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2gmkdtaul.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2rejezcoz.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2hhfcxfnu.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2mypktxhy.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2mjpanurp.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2cstkmcgs.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2ztppghgb.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2gwuxuwlf.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2yeajenrw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2laulwixh.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2wmsnuzrw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wavrcdel.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2rsgauhxo.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2rxqrxbxi.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2dwudgzgv.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2cmipdcnq.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2qadiahhi.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2ehanhhrd.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2zbmvewne.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2vlzkxlvr.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2embwfypk.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2fymmphcz.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2esbqmfkt.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2xjokubfb.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2hrxopnva.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2mixhbgte.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2qdlialwp.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2czfdqjni.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2hijvnxzq.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2ijumpeql.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2jcifxjqf.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2lnwlqiiw.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2ucsydssm.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2kycbnsvo.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2qewajxqf.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2mnrnxfkv.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2rbsmoloy.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2plzvndox.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2wazqhrgy.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2pvyrstpq.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2gibmrdgm.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2uotaefau.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2lowwqybp.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2epspwlls.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2imjjljzq.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2trhxlbaw.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2chohodtx.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wnvmslmz.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2lncxhphy.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2rwjpzblo.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2fwnjcenl.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2gvobrque.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ttvzbxbj.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2tnabsuwx.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2kobrszed.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2nffwqqih.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2sokbajqf.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2cwacpptv.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2pqzmsifu.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2gusnnigi.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2hcfoyuqc.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2wgwumlxz.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2qtptjzjo.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2miqujbuc.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2twvzsrjm.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2sricmxor.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2lqkzqite.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2izrirsqr.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2itytysty.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2vsbzbfzo.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2qcyzkpsg.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2wldsxpct.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2hcdgjows.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2nicrmvtu.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2sspqqhev.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2untfcayv.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2aimomkqz.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2bscrjoxj.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2wredzhqh.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2tqjvpget.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vxyzunse.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2hmjklyuc.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2eaivofeg.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2fcsxdmnq.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2oyhxdrnw.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2rgboarpk.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2uvmfktoe.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2fwmznqgi.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2arwivgra.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2nmkqfzyp.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2dhsscvfw.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2jyoqgmnn.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2wqswqbej.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2wjrkjuoe.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2gdibaejn.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2oemmambn.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2ggyrgqfj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2bnlmfrvd.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2robohrlo.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2dpgorfdp.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2crxevpwj.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2oerjvbov.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2tmfsmwsd.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2kaajyqbq.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2midbpyuv.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2ahbazgcy.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2wvirblic.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2qmmvietf.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2fudqbxvd.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2yezxfqcq.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2fykinamk.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2gghqrimc.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2hsyfxfri.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2smrbbwun.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2wjscqwti.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2zwrdnzbz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2gytquppe.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2ldqkzedf.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2mzuxzyjp.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2dmwhpaii.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2orhpibdb.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2tfvkjkun.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2flhfvofi.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2gugdqbpb.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2akdfwdbu.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2xjswrkry.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2prnqhjje.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2fcwfzzbk.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gcisuaae.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2luxotuwi.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2dimkqskg.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2bxjqtrsw.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2kziovmmn.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2cfcmpomp.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2wznizpwm.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2ydaxodap.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2hmbutmzu.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2dduwrssy.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2poxfpjzt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zfotmpdh.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2ncpyjetc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2avjynodw.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2znsolxbw.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2wzlafrbm.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2rljejheu.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2xcdfmfor.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2hulekoyf.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2ythryuwf.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2tcsextob.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2umhujlue.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ltahizhr.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2enijrpvk.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2otzxtyfn.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2tjrccdlw.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2vjdvurxx.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2sgeuooby.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2lzmkfevw.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2qvtipahr.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2ofmitwmt.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2zaubnhrq.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2bendohvh.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2jjsgyjfo.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2egubbyig.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2lglwvlbw.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2vzmsacae.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2qzzivtef.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2pdjlxqje.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2jtufnctb.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2vlxsjddv.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2jwpynggt.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2vwmmuxvk.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2xkrjreat.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2kndnyfgc.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2xlwurtuj.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2gjzjqqwh.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2wvvljurr.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2kwwgoryz.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2xxtxfaho.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2vgqjkdee.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2kbmkuhyv.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2iytzlinu.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2njcaaway.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2grbdsweq.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2sryxdfsi.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2ckgtyzsc.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2xhvjbgbw.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2jfjrekrt.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2adchvtuf.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2xmksktsw.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2xvvfcyuu.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2kuioqejg.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2reiqwdph.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2kqfkkwpd.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2xxaggsnk.html


<!-- 参考信息 -->