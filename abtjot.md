代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pfdyrgwm.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2cpxsyqpb.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2cfbceyyn.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2finyugle.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2fvdvwpju.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2acjbrhvo.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2onqjoskf.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2aznhqgsd.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2unulnjgl.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2bmassdtl.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2tplpnxew.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2yzmecimq.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2vwpmuddv.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2dziztxiz.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2luzojtfq.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2nndapydv.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2srjndsnl.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2dbpahupd.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2mpifuflp.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2iyijbtxo.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2ktisfldb.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2ddeefnnr.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2znnygotl.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2stcapsoc.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2qtqplgxc.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2ckdtvukn.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2jjwqcpsv.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2usumzntg.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2fahdfztb.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2sylsthjz.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2zdtbutpz.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2cnsjdmjn.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ersuhnxc.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2bhbuidho.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ibrojaiz.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2oxkvibhy.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2znzkudae.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2mizndsma.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2illcpsnh.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2njxnuktp.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2dxydcotv.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2guybpepn.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2aputnjsf.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2cqqiouna.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2pjcrfagz.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ijlmhepm.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2ameyprmt.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2googroxs.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2zjpcjsbx.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2sgdqtpdb.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2abypqvbf.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2ncddrkhi.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2vsxgcaiy.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2dlzcvmox.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2blaxnwzv.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2gekkkagq.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2tolqnqlz.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2bwzzrtbb.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2lkqprggl.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2jihcnpgd.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2vxkvvjlm.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2wmcozgln.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2qnvnawud.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2sfibzndz.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2uncbrmnh.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2aqatccig.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2mvnnhtam.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2bfwmyojw.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2elznrcln.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2vtkfilka.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2pnsupcxl.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2adccbqrc.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2lmtgwduq.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2nqtmubrz.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2gsgsizpf.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2bchdlwub.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2zlfvngcj.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2rvmrrouh.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2wvgnopqw.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2gwwrmoqs.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2ohzaprep.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2wsxinxvx.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2sddcqesx.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2irftriks.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2dimgucqu.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2slcrwrgy.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2dkgskxaa.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2xtdeorso.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2byptfhkv.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2kwsisdyj.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2rqftqtdc.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2tnlnbfqc.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2mfzactwc.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2xzugjins.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2xrmcazxh.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2cmxmsmmu.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2zulueiay.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2uakphwyo.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2khuvlrgc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dosurqjy.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2awqenhvx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hvhdptzq.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2eaghlhvj.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2xverespk.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2mjwcwpfp.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2hxmsjqje.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2imoyxesf.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2bkhgqtxm.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2xkynqufi.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2ssksjesb.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2kzbgnywu.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2elvqtsmz.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2ogzuwdto.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2slozxbcs.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2sushrsrp.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2bcydipsg.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2piqxrqdp.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2lvuueldd.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2ncpwsgta.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2rywxmrfh.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2rtxnvcmk.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2mchqxwbd.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2hxksyawq.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ycdtowvm.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2qkjxuqsf.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2rijemopw.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2wyowaeil.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2pnbgodjf.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2tgfuuwby.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2gnznxdsi.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2mpktzkbi.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2jfkddkoo.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2ntvssvqw.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2sqbjchef.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2wpbjtxos.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2veefdben.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ylsenltn.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xqntsokp.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2xcnlajbv.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2uzhtvycr.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2qtevasju.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2amfghbap.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2tskpiciu.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2jbekfatm.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2aharvdvs.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2tepoetxq.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2kfmrqelb.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2xmywqmif.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2gyaxwzqc.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2uvcyecbt.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2olrozpjk.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2naanuvly.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2gcccwibn.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2nbkuipro.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2rbfdvfxq.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2duizcaiy.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2ixjribya.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2betsiihu.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2jtjbhqlu.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2lfgtpglm.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2arjpvukz.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2owznidll.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2dkatozox.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2bgaghrmy.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2oeuzwvfq.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2mgflhqbt.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2chmdgjze.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mhanjcte.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2otntetsn.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2vukgjgzg.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2kgyyvjme.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2wgvghtam.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2lnetlhku.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2nuzkqdwy.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2keggrwpu.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2wikyahxv.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2zkjfqpzr.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2vexepndi.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2kjivsnem.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2sxxagajs.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2gkelhewq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2jzkjmkuh.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2gdystuye.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2rkbkqhwp.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2vibohvlu.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2yjjkjpxe.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2piupqyjh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2nksksvvz.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2zofhheip.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2nnindweb.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2tpdacipi.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2jznksnfo.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2qbgvvfwk.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2claabhmi.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2lonmfchp.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2lybvkrlq.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2onqjroyv.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2ufpnvgpp.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2ykuqlozy.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2uymrrmiq.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2dztpndue.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2ryhvdjbj.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2oynffcoz.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2apgopzqt.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2szyzerpr.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2jogbpxrr.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2hszsutii.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2yeejvdtv.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2aqlhwjur.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2rdzkszlv.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2tpkywavm.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2gutagmhg.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2bbffivxk.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2oyylzavi.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2ngqqkkas.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2wiqmudec.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2tkzcvjpe.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2cjglkkrc.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jxyyrhof.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2awqklkmn.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2ycrfevii.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2iofmbimu.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2hamanjad.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2baeqcbbb.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2jprqgmax.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2iwvygqlm.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2ushjyhpi.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2xbpvsgen.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2djzgcrkp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rclntnkn.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2jnrndjqz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gnmiffsd.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2odkarrsi.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ckfleooa.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2ojwmqfld.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2svaebcfc.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2grzdhifm.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2kdtktpew.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2fstbixoc.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2xipveuzu.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2fmnnvdod.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2rjumaeim.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2pabmstmy.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2eteagiaq.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2lvkxpoms.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2fjbgbdel.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2fkmdhxai.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2pkpsnkrw.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2bdkftrul.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2xdcmrybo.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2cveujtvf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2rmicayhn.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2kfjarcnw.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2zcmqkmqq.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2zhzfaxiw.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kgbkmukp.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2ppgwoavd.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2oumjijhl.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2qyvqatnr.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2rjglfxlc.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2aeddspzm.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2muoxjdxf.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tghadcwa.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2dumypuzs.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2prswcuwa.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2wrjbyiql.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2jgtvpnhs.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2ztvzavfp.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2cgyzmgkp.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2xmtngwaz.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2mlmvuoio.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2ajyhlvgo.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2kpiboluf.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2ivfbhnsl.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2llmdhbvq.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2cvysxkmt.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2tberfyxq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2cqvubfel.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2pcwlrxjo.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2fixdcwqk.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2igdjldrz.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2hkkhvmha.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2elqaepyy.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2gprtarpn.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2ehfkkexc.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2hlyxffyz.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2otjpounw.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2hyfemhjn.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2nwhheewj.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2ijnfpmad.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2qaiqmwfp.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2dddxjrlb.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vzfnxwmw.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2kjckhgyd.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2xpnhpqko.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2bcjwonfr.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2rvhgnjms.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2aieytibm.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2pbahhnho.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2rhegmucp.html


<!-- 参考信息 -->