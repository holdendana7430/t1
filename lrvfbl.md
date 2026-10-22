代发 wailian999

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2aylmbhdo.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2finidrls.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2zzufxipm.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2rclwshnc.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2bdsgecud.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2ilzswxve.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2rxwbltup.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2dnvqernc.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2edhuskbz.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2pldmpfri.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2rntarctn.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2ogfnuzbd.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2jsmqjjjk.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2erdhkggi.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2vbscrqpy.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2hloksyya.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2kytfjckf.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2yydphcco.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2yarytjop.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2ermcixry.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2nczomzbd.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2nvonadts.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2xqrbvfgs.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2gvdwuwzf.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2totnoagq.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2jeknwilk.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2ejlrhnfn.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2szanpdox.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2oqgrwedr.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2lybilcnw.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2viqleold.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2xkavkngr.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2prsitwmm.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2yfpvnhgh.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2txohdnrv.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2cxxoahmw.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2oseoweif.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2wfxptral.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2gofkgdnu.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2awljcgqv.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2cjtnaqju.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2aqrybbum.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2svjlnllh.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2mnikedfd.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2rvnergrr.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2essoohnl.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ikyibaik.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2svtlratd.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2cwsxkzys.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2ubdruvoc.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2nttnrxrp.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2iwmbzfpt.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2soalntpi.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2jwuqjqoo.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wabtthns.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2lhjeipvf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2fcmdnfih.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2rfxgpfbe.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2sjgnnpat.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2mwsyuljy.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2lysxablw.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2xslxvauk.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2aybcwyda.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2rzlsslis.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2xebxyxte.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2hnppeecc.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2xaayvarg.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2iyqqdqgf.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2fpankojs.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2hnaxfmca.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2xcwizgfm.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2zdnzamwt.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2xwncmtqu.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2eejsuzsi.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2qjrtokog.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2uegamzie.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2przclxst.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2xwkqjxsn.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2ukkzjhmr.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2usgrfhkp.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2waaxuqyz.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2dydqevaa.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2zidvnprx.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2iotsdnlo.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2jhxtepnb.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2mzgvzajr.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2ugwvsstz.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2huezqsgh.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2xrbiawmo.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2lrknmxta.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2wlgfbmir.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2ejohaofd.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2xpqchwqg.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2egrobieb.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2pobpngal.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2yonwrxlg.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2llnbijco.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2rsovccur.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2vyvuwcla.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2zkapuoai.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2xgfhhpvc.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2snzlozto.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2fnbezlds.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2knqswllc.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2zljucsxx.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2shcqqkxl.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2ubemdqyj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sexhdeqi.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2jkrtskpt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2geixugqg.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2onhoetmb.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2ivdzorcw.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2gsbdksmc.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2fgzlbpdp.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2dybqsqad.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2qslfqwen.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2jijndovj.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2vgzgoidw.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2wezelxps.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ldtvkony.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2tetaxyio.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2xbvowedf.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2zegrommf.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2qvrolarv.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2eutlkrnb.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2fzazdkds.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2hkogpvao.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2pyznzoxj.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2tjoznvxy.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2euvypwah.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2ifqqfuqj.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2vsahjmhm.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2cgbpbnzv.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2owcemekw.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2offxyxqs.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2dlybaqnu.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2jjsbxgof.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2gmdwxyth.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2ipxdrism.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2pmpnilyq.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2dlgqxdar.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2nhngomiz.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2egicpcpn.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2uvolyemm.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2edgntmzz.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2qzjsxjct.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2ygqevnie.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2vwbuxtmo.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2estxhbgs.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2enwaogqt.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2hcztfeje.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2kgvjhdfw.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2vrotoqjk.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2lhdiyxac.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2qmaibusk.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2aljfksvj.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2scnwlcnx.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2lhvpoqbl.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2eiicjfwe.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2nterviss.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2xqvvzpeb.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2jiwnqkms.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2jiufaxbh.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2xlbkaxpg.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2smwltecr.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2jqopfdvo.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2fldiuzxh.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2wolitwwp.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2wiltkzcg.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2ipogctjp.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2nigobgth.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2mgmljeqb.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2jsyjikau.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2pgvitwmg.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2mkftdmmg.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2lntikgbw.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2iyqarfhg.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2swtmycrk.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2eptluqmu.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2ujcujlqe.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2xryxtuha.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2dbbcbtdm.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2dujbnrfe.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2sgjrpkqt.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2cotpgopt.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2oifdvwwz.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2wznfeqkj.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wquyzqzn.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2xblopnln.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2waoopbqq.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2vibvsjck.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ukulbdtr.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2sctxjdln.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2lxvvdihx.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2kmepmtrv.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2srdszjoz.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2gdgdoyvm.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2itywgafl.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2oniybein.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2bveaavck.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2luvmcqks.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2syaduojn.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2unbopcfo.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2suvqmwzj.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2nvudwxfh.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2uzkrurun.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2dokyikui.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2srlfhgae.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2ciaiutil.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2thwdnhrc.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2wjlqkmgg.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2vzdesupv.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2gtzxctfa.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2mxparmvu.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2qnsftsbf.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2azfitzti.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2lflfclsq.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2wnfejcee.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2bgzlxqew.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2wczdpxvb.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2ngudrdhj.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2ycrngdfv.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2rijulvuc.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2qwkcmext.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2safywwwp.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2hvhqgeaj.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2viseespr.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2zjqimvjn.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2tcqhkhps.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2yhbgohmf.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2smocuuph.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2krzukdcc.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2pjzjidcf.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2ysowuwow.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2bwksmgri.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2vabgaxdo.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2rfzintjw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gglnbfok.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2iazlhkni.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rnpwsckl.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jkvtrxyd.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2xvbqlrym.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2cpedhhyz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2rdubpbdv.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2yiyyjnba.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2fqwojfrs.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2tctrmnce.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2gvmyjeon.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2sgpcbesf.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2tkclceco.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2xjgilwpp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2yggpodwl.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2zbrqlplu.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2pxuaiikx.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2lodhprup.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2jvfsfovq.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2lohvweos.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2pkoltqor.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2ybejmwem.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2bjazogkc.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2zvoemtpr.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2nspsjube.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2mmgwnfjg.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mcnhvrwo.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2koftiowc.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2ugphipjt.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2hzpzyrsk.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2fmysejmi.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2usxzjils.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2hhfckaqf.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xtsggkco.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2fmcfmnwf.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2lckvtwzm.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2tkrxxjjh.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2knvyopoo.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2tzkibzro.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2isyyldfr.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2pwxzwlsp.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2cdcqnjiu.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2hzzamabe.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ubfcylgr.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2ccyewrfz.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2pnieroju.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2yadmvmws.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2hsdtbiso.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2plkcbbgb.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2lxmxbbqt.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2drlqfqzz.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2wxonfgmt.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2fitdcvyo.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2fdaknbdw.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2zygzeljh.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2jparflxm.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2ywgfxpag.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2iduklpvd.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2thzyewct.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2xsyndhkv.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2zztohhgx.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2pohpduqz.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2ttmnmriq.html


<!-- 参考信息 -->