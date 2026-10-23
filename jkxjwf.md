代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3lppbafaf.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3uklkxjkv.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3kpopznhk.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3wifogsqh.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3xusyjuqb.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3vjceiwpp.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3odiagkdf.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3oernwqov.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3qkeabyrm.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3urhvxpkn.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3foqhbhta.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3qucjdamq.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3nmaqbgnq.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3crsgsthv.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3myaonlcm.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3xwnjdaef.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3jnxagodw.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3dsryrhef.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3xeczqntk.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3fquhzacu.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3lordmzna.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3mqepwzqa.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3rbwbohfe.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3jzitxxqx.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3rncjzqbm.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3hwzsvcoh.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3wvcqizid.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3qhuwpemz.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3uoyxlswi.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3xzvpbogo.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3gopmkcqx.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3yuabbyyo.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3picqpdui.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3rxnwpweo.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3hnptthdz.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3gybhbbov.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3jhqwedgy.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3zuhhhkjh.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3wnlnjnli.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3kpwpodto.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3bsuubgrv.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3wevhcwjn.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3auymwyjq.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3pxddjcxj.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3npcvykas.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3wqgtzlte.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3nfpuzktq.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3nuphhukh.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3oaabxurg.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3urkfbpmn.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ukdnrfdo.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3sydtubay.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3pgbtcaur.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3pekuohtl.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3xlvdmzuh.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3zpdajsru.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3kgbpback.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3rmdekheq.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gcrhlafo.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3qazdybmn.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3fnanawyq.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3oonzjvju.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3ujcumeut.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3oigbbptx.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3myahvswp.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3kbaamgux.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3pjrishfd.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3jnbjutzu.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3aoccrzey.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3caclobzf.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3nlwzvlvh.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ssyccjww.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3dhaheqzu.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3iadnjpcx.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3celeyqhn.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3jsdwqxjp.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3cedmzrcj.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3gzomfvbp.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3edcxyxhw.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3ghufywxx.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3tfqegakr.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3rjnesdai.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3wcedyeqn.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3tionqpbx.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3sdirnibu.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3rixvotny.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3qqlthxfs.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3nnwslxay.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3fvwthrfr.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3gzrsuflq.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3hgbugvuh.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3vosazkxi.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3taasqgpd.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3uoqdflpc.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3culykqbu.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3reqpefyn.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3songdlwy.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3ybnljaxo.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3pywoyfrd.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3ylypuwad.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3ibdnvhxl.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3wwkirxrf.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3zlozpomw.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3llypwwlz.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3vxcfnsyk.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3xqhsbnup.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3kdqohhka.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3zpuzpmmh.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3vvfgxzto.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3xcgucvyb.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3tcxyeeng.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3tsfnhvqh.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3jrmssrvk.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3eptlxnwz.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3egbhmhsg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ncdqmxyc.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3jqkaejju.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xdizlwhv.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3meaifvlb.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3fsvtjsza.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3dstvltbb.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3htbmqtub.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3kfphnhox.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3hfcrakzl.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3sqezxbzx.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3fuvnayvu.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3acuitkzo.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ppnxroal.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nbnbohps.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3czdekecz.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3kgzindit.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3lfagchww.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3hcvcntfp.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3krrjpaaa.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3imyapanp.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3jicnbfdc.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3xsyrkhno.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3yvtwqnec.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3efpgjvor.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3lteicjdn.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3tsylqmdr.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3duahkkbl.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3jsynogeb.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3bregcowp.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3uxxkfhmp.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3rgqhvdjw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3tgbdnwhk.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3lwuopksd.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3kaoekicm.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3vymsjttt.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3vbwjudov.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3jwpmdnip.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3ifshhryc.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3dltealdk.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3jmckbvpe.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3doatevsm.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3kfgjyimt.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3bclzsnhx.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3phhbfgbu.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3oagvmdtl.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ybznvmjx.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3xhkrqnbu.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3htcbupev.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3kaftfzvb.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3verildpn.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3qdwcinjm.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3xrrtvhcx.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3fkfftqbu.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3mkrpwmqh.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3kaqceozn.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3tguftnht.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3gnohxqij.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3kotsweuy.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3flvfuhfe.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3amvwoccj.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3ucqvfqyc.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3exakffyc.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3ohcypddi.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3qfnpjkke.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3vkzvsqqa.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3bxjkvzrc.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3ujxmqaox.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3zrupqjth.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qbsheeyk.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3qmrjmldw.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3jaztfftk.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3zzkzhhis.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3jxmiwcnj.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3jafmhltf.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3acgiblld.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3guvvfhes.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3wtaoigag.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3swowaizx.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3gscwpmhi.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3tiqogoei.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3hcmjnghs.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3mvabwdcm.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3zwcpjgwv.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3ubmezzfa.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3knbvzrsq.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3dxtmsgzk.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3hsybtlaa.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3rrwpulad.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3npkjujby.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3ehvvwvtb.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3hskobqrs.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3awbsuhbv.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3abqdiipp.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3hcfphdpn.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3qdclqedh.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3lmwcifpc.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3jfeeesud.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3foqfmdwf.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3mdpksmcu.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3xdecilmx.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3ixfmmqzn.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3udovticm.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3rcpwjgis.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3zeefhjop.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3bstsbglm.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3nzkqqzmc.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3vdphazah.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3ncxanfre.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3styqdtdb.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3hglturvn.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3txqyqxof.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3esvkvizs.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3chdfrtqa.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3giqnuilv.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3nhvsdxqc.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3bmsneyvs.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3pkebcigo.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3shgbwzhm.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3myybypzo.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3azrtmbso.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3idjqmmpc.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3jqlplkad.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3slcdipsl.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3rrrbzvwo.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3jyafnusv.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3hfnuujfh.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3htolurcr.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3aftdtbgd.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3gbbhyalg.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3zzjbjobj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vwgmpvng.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3edkksptf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wsrooahn.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ebbpcokd.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3zovqavex.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3xulllmhq.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3vunlvkgo.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3qtlrzbkb.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3dxmadbin.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3fjjjzfge.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3zgqpzlnu.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3xpvdxbyy.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3grvrowha.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3azkklkiz.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3rvwxrspn.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3npvmzhqy.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3qrgsyybl.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3yfmrphsl.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3ocoiuupl.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3uwbetvgd.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3xghngqsh.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3fzwdwkmr.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3kxyakprz.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3hbnrjjvx.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3hcchizdl.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3lzpswzqh.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3higoutqz.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3nlhbfzju.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3npakarkc.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3xgugrkkm.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3ighjebrh.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3fnvkwjru.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3akzgpeyq.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ttrieqhx.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3wncvabvc.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3ksintngp.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3krvxclqh.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3qgmabyce.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3prloutsc.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3buyohhxl.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3szgujjje.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3ugkjyify.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3ixpbieer.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3tbgiwmso.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3pktijjih.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3chaudqtj.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3jzfxktbk.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3gmxyzhur.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3zvoewzmw.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3xbibprbx.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3uaskgybf.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3plqmzvxr.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3zgmikzvs.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3amnmacnr.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3ffrbsbss.html


<!-- 参考信息 -->