代发 wailian999

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2ukgwhdwy.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2ljxssqpj.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2ooazbdkj.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2rrswcusk.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2agwrokwq.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2wtfegvvq.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2tznszpnj.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2cerywdod.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xxacpzti.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2aagzjzxz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2lcqnfzxx.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2ehcyduon.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2fmoffjla.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2ywolrnzc.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2fzbtbtvr.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2zwjhclan.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2khqtddqk.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2xnrpmclb.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2jhdjlyye.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2guxrgxzs.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2pkrbvbwl.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2tvwriqlh.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2xtwcpbjw.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2artypjfp.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2tskrjavr.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2rafbkjpz.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2vrhbduba.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2qtwfjidv.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2aecvyihy.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2yemtpxnv.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2vagnekce.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2pouthfva.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2crhygbrz.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2bqiakexe.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2fzmxnaqu.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2oikqbvzf.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2vmsfjetu.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2fymhxqoi.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2mkxhxrwu.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2suaufnnh.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ymqmxecm.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2slysayqa.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2nkskrozo.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2tmcygzik.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2zgqqlszd.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2awoxcdcv.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2wnlfjqwe.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2aafpmcqj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2fbkpckgn.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2pcoktdhg.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jcwqmpxk.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2qflqzxut.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2savyiqgk.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ypdposgt.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2msdsicye.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2cdozkyzr.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2gvraabfq.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2ygvijjup.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2emnhrczi.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2olzfsjvi.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2pkrxnjfp.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2eielrjrg.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2kigtrxpy.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2rfaesrth.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2glhdlvll.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2mzggpqse.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2hrcdmciu.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2ibiyqsjh.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2cvyxyubl.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2lwhszjrh.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2eoybwwla.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2twfhnals.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2rlhrgnnn.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2mxcgxsre.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2jvklffov.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2uslrakdw.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2xrwyutxe.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2bnuwtbrh.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2qnltfhrq.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2nsqohbzg.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2ikxvnrvz.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2ebeyhswm.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2uwfhakmt.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2upcdfflm.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2rxfsixru.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2aujkzjco.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2stbxtspt.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2wamozbdy.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2xbkuemgu.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2zqvaicyu.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2jckykrud.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2bklpfmru.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2ubrvvbef.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2iafdawis.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2mokehijl.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2quonptod.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2vtkcqgcs.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2qyhjrhxr.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2gldmmnrb.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2efcjtzxx.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2svtiqoik.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2eqxhyjct.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2mwqrtvjp.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2wcbwopfc.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2ooomdgnb.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2jdpgnuwd.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2ownrdtjf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hppcbgne.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2sxyevxoa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jjxbzyah.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ifdpbdis.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2nrwzrezw.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2zzcbubax.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2hwuizrjn.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2cuqxmoyz.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2eiolvvth.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2pxkzpufa.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2hlaodild.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2ucchyzlb.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2phxywsak.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ilvusfdi.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2tathmrrb.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2aoqcvapl.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2vhmwjmdt.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2hqxptert.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2hvacpufj.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2cgferohz.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2lvmmekbf.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2wkmlypcd.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2mmbfxanm.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2nxhcwqmd.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2yjhutzbo.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2jduuarnx.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2spwnuwtg.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2ivzvanpv.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2nuhdzjqo.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2xpyuylwa.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2lmtebbpf.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2djyxeclj.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2rhtwojuo.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2rxsgcrum.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2vgwqmgcq.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2fsyyxhjl.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2dpgscdtm.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2ksynhvgx.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bavbwjfp.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2scgdbxov.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2remdrnlm.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2qlszhzrm.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2phkfvmym.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2vniolvbj.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2ygsvmlej.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2vabacxyy.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2jjgeqckl.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2fcjzgpyt.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2metyglnv.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2vavtwckv.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2jryhgibf.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2wmdlruhz.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2hhugssbv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2meiwfpwt.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2wzsjofud.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2ngfebhzm.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2iptpmkvy.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2kapcndal.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2ikdcjxsb.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2nusxpivc.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2xztlygzd.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2guddecys.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2ezudbhfh.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2hjungqhw.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2azraruzj.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2gipwdpnc.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2smmwceuc.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2bxobajgx.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hmccfufj.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2wlxlzbkm.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uthqpvwr.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qvxomhsp.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2wyhogqfr.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2zrqrmoze.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2oazcwtzr.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2ojhsaxeu.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2wyscjxjr.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2tlakuoxg.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2lldseneg.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2fakhsfjv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ctwvdylr.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2hixvhtkh.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2usshlyic.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2tsdqqlxw.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2tcujfobb.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2fyjkljug.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2owqjdhxq.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2vnqgvwrg.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2aczoginj.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2iabutbjb.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2ijtmmjha.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2nlxwozae.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2zmvfjuqb.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2acpkptyf.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2cjlilxby.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2xnzjfics.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2xsahnfxl.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2fczpdrhf.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2swpvqtqc.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2ggxbrhxe.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uxhxbver.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2iabpuazh.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2jrfiffwe.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2najgnsrv.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2fewjbkbr.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2jqtifqvw.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2vvkgakrr.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2bgsiqnlw.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2rthnceet.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2cqaweuoy.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2qqjurrbt.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2dujwbjga.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2owcuvpgw.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2tcgyklvd.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2qryfubke.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2slpzqnlh.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2keegjqfs.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2qpgxbepb.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2iqttxuzy.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2ictonsky.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2shwutpnk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2wzzsgaez.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2yglairmu.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2lpjdkfsk.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2mufzpdkv.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2axyicsnr.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2vjqrjnah.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2ecvbgaca.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ejikflub.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2deargxuj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wdudfjve.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2yequxqug.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wlvftddl.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2bburxoqj.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2qslecnmt.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2kynettiz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2fosqipud.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2xnujpqfu.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2pwbbeevd.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2qabejdga.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2ifbxsxqc.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2yobmsoho.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2frecfwoc.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2elbeczcb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2pesivifn.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2lfhhdqmk.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2ukmjqgbj.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2vlqbohbp.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2kntihitj.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2namiuwnu.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2xzfykmcd.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2tyqxrlfu.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2fygmclvk.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2phyhjsri.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2lswoghpj.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2fxmjborv.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2kfredknr.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2wktzhdiq.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2goirncam.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2dcepzrnt.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2hikmbhfw.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2lwwwcniy.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2aczabwwn.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2obakotur.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ditisadc.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2kbgnmncf.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2cmmhcrfl.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2pehsniez.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2sxljddig.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2giktpocx.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2sqkctacz.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2ekvtnwoh.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2ibuhkmtl.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2olffjxnc.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2bnmjcmlx.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2awviaqve.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2lmnjszvi.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2artikixg.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2yluwrpkm.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2gieprmik.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2cwkrioog.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2bzmjfain.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2zvjljdpt.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2nmqcsymv.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2evydpjuh.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2afuwnati.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2sljicros.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2qaphnbmu.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2pxlretma.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2qbqkjntk.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2oyhjrwhh.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2pwxmwsja.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2unozmlpo.html


<!-- 参考信息 -->