代发 wailian999

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3ogbrsevz.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3xdveysqg.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3pxpetadh.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3cfzetrid.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3xrsukovk.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3yqfcywyb.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3uoxyniuh.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3ubhnftkc.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ankgviyb.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3qeryofnt.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ohwjyodm.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3szfglvax.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3bsivpdoz.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3ybwsprlr.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3ofzctyuh.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3louvpoaw.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3rkknjoqe.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3kwwombwt.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3cdpvpvqy.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3dzwxfkor.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3pkojtlue.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3yhuczmba.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3cbzvwsoq.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3ywtkpcqg.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3fajnldfk.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3miogajlo.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3ugjhrksc.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3xgkiixyj.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3vbkbzgcr.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3rabljibh.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3eedhujqp.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3gjytdvct.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3cuziauaq.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3vgmylggq.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3infooinv.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3aptopsex.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3pxferrkh.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3jexjxvza.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3bglhwrot.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3jedpcplc.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3pmirfsvj.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3rsjjnmao.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3blqbrwra.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3usssrdmv.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3tdyvjxtv.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3jnrltunq.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xpvsjiye.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3mtkyvdzi.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3lhpmyfts.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3myjvcpqa.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bzfzqriw.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3aminthdz.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3wjibnpsu.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3tklkxwnu.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3mwujlejg.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3gbgbypfi.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3geqczrfu.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3xehryteh.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3ogydxchw.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3jvqpzjdf.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3qzwzkkdg.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3tgelonyd.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3nruamdku.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3acfxxykk.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3llugxpaw.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3ojsydmeq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3zhgwxufk.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3cesokqgz.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3txduugln.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3lxdzbyns.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3rpfwrodj.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3edkienfn.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3pybdevjk.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3eqdcxgqq.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3rihgwntz.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3vqpmohgn.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3pamrfthd.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3jgfdpzru.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3oddncbqz.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3hxvghqjm.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3foxvkhoz.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3ogdpdgfr.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3yvrfadsq.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3otpaewpc.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3dyoysgfa.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3xkxwlauh.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3iimiisgr.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3mtyoohdo.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3lntstpsr.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3fsvlbugg.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3ivmzyxun.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3hqyxcwpy.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3cgewupxi.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3zejqpjdb.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3mzzrlgog.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3hkajpwpt.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3fhxyfaeb.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3vrcsqyci.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3baivnygo.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3nbxtxdfc.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3mrebmubi.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3qgimkinn.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3vafztxqs.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3rfonbupc.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3xqgeljmg.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3ptwgfxsx.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3hvxthjsw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xkfswztp.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3jhrfilyk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mjnuygnd.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3akwjbrnx.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3cyqqsnur.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3zxdzamwn.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3hmfzgatf.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3jacatuyi.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3vdtsbqyr.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3edczgfhm.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3acuanaqw.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3lorrmouk.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3vulbdqom.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3emwyyqfe.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3pyfjeldn.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3zmovexdi.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3dddgysch.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3kczjbcqr.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3zaqwnrgc.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3oilhuznp.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3gfdsiglp.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3jyewchur.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3blrtivhe.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3zjqcvcho.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3gyyphfkn.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3gqsovrrb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ruoupmcn.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3mrdocvco.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3nekrjuln.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3hfaszosd.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3cslgxafp.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3niydfssj.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3yenxugrs.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3czzqfbrn.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3psfezepx.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3yjycyjhn.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3pclpjzal.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ofztjkxn.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ovfnwcys.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3hqkjkmhg.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3hvyctfws.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3hzvzorsd.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3lwafgfyk.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3lcskhacx.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3occobpul.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3qdcyjpbs.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3rzzzwihp.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3ixlwooks.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3etcixwhw.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3hhymxulw.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3bhdpzpre.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3wdvhgpxb.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3wfhkcvof.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3dtdculny.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3ofeljsoc.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3wvgtbqbz.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3sxynyrsf.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3uioipihc.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3glwllsvt.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3snwjnvwy.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3tjdryktk.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3indalwjb.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3liepjoso.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3ledtyorj.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3hyaxighu.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3olbwzfnb.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3asuzagep.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3prtpcloi.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3uztnmjit.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3ehhlbrva.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sutfryho.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rflujqms.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3aujrqwgm.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3rzevcfbp.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3cabplvrp.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3vyhgcztp.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3anoqffic.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3hukvgopq.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3mowivvxm.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3gaxrquux.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zuhgdfuq.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3ruohfqmk.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3turdliqh.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3wszmvkeb.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3fleyuwqu.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3wjcwjglu.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3gwodfxtu.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3wewjqodk.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zdwruqcs.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3qihyfdcy.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3pekqijhr.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3whlsdsri.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3hgbsjtqo.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3fsyufjuq.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3rxvamsfu.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3cjumqosz.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3hgzclmlo.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3itjlbtsr.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3xjoxpgax.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3fkpcpjmf.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3iymldabx.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3liftllbv.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3hzvdufac.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3egqvtcmb.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3deoaygqn.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3hzdrocvv.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3dnpjrcha.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3upyibtpg.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3vshhwmkx.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ipxtnsyc.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3zmekdfcg.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3giwwfrzw.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3jqfxpsjb.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3thuryiec.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3cpwceuvl.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3hdesqtyl.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3lwgzjqxj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3jepzlvbq.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3irwxoeue.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3tmjuhxeh.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3hqcrlklp.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3uqkgfyju.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3rjsjgvol.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3koyrvrmp.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3aqbwywdt.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3jirzjuoy.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3ywwjpesb.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3bcdyipig.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3tqqzeyat.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3wlqarpwi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3clarqnzo.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3uhipyhew.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ujgbmzcp.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vgrkqaae.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3dhdpdund.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3rwneeskv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3hnrnfdob.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3shnbhghs.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3mwjcnloq.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3eqnnbsst.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3xsgnuabx.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3mngmgwmw.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3wmzliprs.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3txaupsrh.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3zoqbeyos.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ggndfyiz.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3iyyechzy.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3shomkodm.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3hhftlyzi.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3kqqbkznc.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3iqlsudxi.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3ytlzmwdg.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3hjzolmnl.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3pjerolco.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3wwapyllv.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3omlyeeey.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ushvcqkr.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3hnfstdks.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3yabxmquw.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3wujwdjbe.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3sqihsytm.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3efnsfbfr.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3idaubutc.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vchnjkgw.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ukpwrjxy.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3ahqtaats.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3uhsckttk.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3erkpcsof.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3fwuvoets.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3kpmuudbq.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3hgphhwrd.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3psrwwazw.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3zkijhjrf.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3npqawike.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3lbejjiqo.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3nlvprewm.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3npxuksuh.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3rmtdlwyd.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3wdnbtnho.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3qbyyhbre.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3lgrnkbsx.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3uqrvvnzy.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3ujtbgyjn.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3fgocvdoo.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3jpouomgt.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3jspjmezw.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3fazrerey.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3aiygneiz.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3hwsgsgjr.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3chovmxuq.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3rrscijxj.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3tanpmooo.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3ukkvjymh.html


<!-- 参考信息 -->