代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2dopnsmhy.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2wusqmgog.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2ifyoxeub.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2qdekkauq.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fsalmfbt.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2lmebolep.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ykwgvcwt.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2yskhsxmq.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2qlxnuqib.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2kzlabtrw.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2oopcxdxl.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2ruszvwhi.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2pcvfptdw.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2yqiyzelk.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2emiitexu.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2sdjvrqcx.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2asdslkxo.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2zjfxbesj.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2okwmbmcv.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2nnvonogc.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2slqkccxq.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2nsvwyvsz.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2ligjkeyr.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2lazvexxk.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2cqzzmzan.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2qirrzssq.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2wyhjzprb.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2gvevkwqf.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2evixpsks.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2mbpfylxt.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2setnxemp.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2uhpezhwh.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2djfwhjfx.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2sceizxyq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2zeedytqm.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2atmrqkph.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2mjwnqavh.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2veffdqtc.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2joafipdu.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2shvnhuig.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2eahvecmf.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2vndxxqyq.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2fxgcbikb.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2njtzttsp.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2dpwzubbc.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2nneiqhvh.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2nuztnyeh.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2hhpokuyi.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2wejvkfxc.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ogfqokhr.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2ytsagupp.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2wvlwqgky.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2komihcwv.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2reocdtnx.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2ylgwuuct.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2cjxlofpj.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2srypknex.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2rrrhwxmd.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2bopzmtkh.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2hufysfyh.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2pmpfswka.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2gbjuijnf.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2bdtucyex.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2qwjsdgfb.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2xhfzoeaa.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2euupglic.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2vsckvhka.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2axsdxhhm.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2cqyoctrt.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2jzjbknmd.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2pcsrarwr.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2cawovtyx.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2elxqyyzc.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2dnpkiype.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2gfpinlqm.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2bxzumsyp.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2wntdqgzm.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2gpmbnqjx.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2ukdugkbj.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2vvnuesov.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2slemqsyo.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2pbryuzch.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2hcsgxmea.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2onhqnqjp.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2tlhpismr.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2fxtaekei.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2xwaxyahm.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2ffdtwhcq.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2rzxdtgpu.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2eprbxxwr.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2xtuzxuwj.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ujwyikjl.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2fqhbmrgv.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2qqhamefn.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2kxrzaymi.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2tdrvfwmq.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2gurtayns.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2rtfnuwwo.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2ezqmwjnw.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2ertvcnhb.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2bilvgeci.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2ogjqsfrj.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2ingbwajq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gujsnqyo.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2mohxxxli.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ngssejet.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2nzypsvmk.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2gkasxeis.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2bbnuwzha.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2oeyrfuci.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2bmaxookd.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2nnaawpdj.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2stikcuoy.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2cvvoapie.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2iighdzwt.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2rymbquzj.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hjtljxtk.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2lthoucgd.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2lkqquvqh.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2yvcjprnt.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2aseewowt.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2umbxbftc.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2wdeqtoui.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2gjnqrtbc.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2wqjqqjtn.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2srydclnc.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2jdirrdnz.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2xpilneqo.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2pvunuoxg.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2paglgusc.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2wytjhckl.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2wlkfuzsm.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2lzgpyyhr.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2zohcsrsn.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2enovrzvi.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2nblzotws.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2lbhpxmmq.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2yirszmqi.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2edhicyzh.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2ijejejiu.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2avvvtxtn.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ydyqydkk.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2ekwztrzm.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2qgljbsrh.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2yufcbjmw.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2gmeccrve.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2johmsyhb.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2bvxjfadw.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2njuauhhe.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2nojhhrxj.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2rufuwhtp.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2ymbkaila.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2pxbzwfuo.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2ydxuvwva.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2eptpyftb.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2spapvdns.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2nggllrxr.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ahhiytfg.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2bykizflu.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2wtqdrtsr.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2tfawouca.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2wyzqwgcl.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2hqujzfrl.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2pxosnqco.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2aokcgecr.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2flhpopmp.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2iqprrzgo.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2drvmbarv.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2uhfzslri.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2ccalptru.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2ezcbbjmi.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tzpkiisv.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2eidgwbhu.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2ltzeucks.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2fgpbrolh.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2ghynakmk.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2ozjetnyi.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2kwzjvagq.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2cnehlhql.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2lskjnvea.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2aawjczpm.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2hahturhu.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2azkjwmqm.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2powmzhzj.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2bomriqei.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2brlctiiy.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2fyvoriky.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2xqxxvayf.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2psraasuc.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2vetkbbsc.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2lbkxwsdq.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tvvqqwlc.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2dihxzacu.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2tsxuuahm.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2crmqsipo.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2wnfndxmt.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2jipzubzq.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2zxkbqbcd.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2gpipfztm.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2dovdtyrs.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2jfdeoiwn.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2ervahpjp.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2njlehdkj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2smdgqnwg.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2khyahpyn.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2ggiocqtf.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2zcslfofx.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2kalsnemi.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2acrqxnei.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2pzzkczcn.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2nxoocwlj.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2zeioxzmp.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2oswjidfx.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2jsxyxaup.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2vgzvhspn.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2fjfzraxd.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2qxiavyjf.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2psavmusc.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2actstxpr.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2oijbmcyl.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2bybiticq.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2ayxqzcle.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2fnsyzxbz.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2radhgtkz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2dlbbamaa.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2oxtfmuib.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2mmyyqikf.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2ldowqphu.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2qkyqiyij.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2vypeabkj.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2ckoxbioa.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2xljimjdl.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2yrwpmiyx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2omzhtjvc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2xtwhnkmg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2skonjetv.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zgtdrrmk.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2krpnkewh.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2xkzgzbjg.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2fqaovhed.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2lrvtotii.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2osymmfol.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2ypyfiyyq.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2qnavuxak.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ckkvfpax.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2udkmabve.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2tiyvgiww.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2kbcksvvz.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2zisbzoth.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2tqndnbnk.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2xohjwnjv.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2fjnjjxhi.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2rrebilun.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2asobzzzf.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2wuvtgpgu.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2wdaoltjg.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2zazfeegg.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2frngsxho.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2lbklnenv.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2boixyhmv.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2sydptlsm.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2suogbuuw.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2ekofondn.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2swkcwesu.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2aqmteqlz.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2fqwpzylm.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qdityjuu.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2pvufgkcx.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2ojflzsqn.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2dvwnxkxd.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2juzwzdeb.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2cumwqhcz.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2rpnbshcs.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2ajsphyuu.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2flcmcajg.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2ruitatqm.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2ufpjtlxa.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2dawmaijy.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2aeamvsun.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2icffepoz.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2itrmrwlt.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2xvtosgvs.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2tmawjbta.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2kuntmaxw.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2wdvbwbxb.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2sqwsvunn.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2helyrjma.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2roghdlrt.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2czuqutfl.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2akcvxxrd.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2vztfnqri.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2wlkhiksa.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2qhvuyeax.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2wzlkmtem.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2wrdxtojm.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2wfftyvqj.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ggppxyta.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2eesnaxjw.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2ycakcbnh.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2rdvzhebn.html


<!-- 参考信息 -->