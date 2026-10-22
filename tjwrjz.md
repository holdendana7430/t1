代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2iiayuycw.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2ztxyfhuo.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2rnktbsxh.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2xtkjjrto.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2bwarcvfb.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2fgdykwyu.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2reulgice.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2laowoqdk.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2lhubmciz.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2afaujokq.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2rvngmyvp.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2himhdusx.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fttbjblk.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2pujocnhd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2bnfnbkgh.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2pvnyikui.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2mcoasadf.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2hwnrdbap.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2kirblylq.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2fghtskey.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2ltzmiwgg.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2suivcujf.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2iceueypz.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2abxgvrjc.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2nnpryxjb.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2chhwjkgl.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2xeiphudq.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2rbhvydun.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2kjavlewm.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2ojscnumc.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2anyykimg.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2kpzilbfd.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2pacatbwk.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2fksyjuaq.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ndpqeama.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2xankzher.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2pnnthqbr.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2ylhguuqe.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2xoszxbvw.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2nnjvnkjp.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2waevivsu.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2zervghbi.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2pcmzwznv.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2ywdoyqnh.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ubxxfoxd.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2blbiqfgx.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hehhapyg.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2tofxokej.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2jkhbniwp.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2vmcwygqb.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2uhvcyclb.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2hyrfbqzp.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2qwgblhxr.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2arvctutu.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2vypqqymi.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2gciuanqn.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2oanucqru.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2rnebthbd.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2uwdqcwxp.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2qsculdes.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2fgrmwirw.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2gmxvgxiy.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2dnbecdqf.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2zzzetnxu.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2djpobmlu.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2txhxpruh.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2ozrzvwxj.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2prbooefg.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2wodsbiqx.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2cfolthca.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2vitzbuiz.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2zrepgtfx.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2lxtegeef.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2dtacaoad.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2jrcibnec.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2khlyaezg.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2iiocevol.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2gewoqhnd.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2vsuhdkpo.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2tttkqdfx.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2fsfbkbuq.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2bpoxdwjl.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2odgwpija.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2wptjflxo.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2vrdgyrem.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2ttzdbexi.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2zpjvahtk.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2cosuuugm.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2axfrwuej.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2jdvphjsm.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2ywsuyvuk.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2csnkfxui.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2wjwtzlht.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2znyncgza.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2jamshdcr.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2mncekcxv.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2dnzkties.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2tcyhdqnl.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2peqjorbl.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2mfyxirkg.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2amnzyoom.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2whzrcene.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2nlqtzvsv.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2xkdfxmrv.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2jxftgrum.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2jjchvubk.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2gjnxpjfj.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2iqlqnmll.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2ltdlojtl.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2skspfmzv.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2xbczcaze.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kitsmvvp.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2ymduvykk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fejclxms.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hcnoimbp.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2auwmuwzu.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2ilswiglw.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2knjbmwze.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2nprgfzzf.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2rwsjjiot.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2wnsevjft.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2jaakifxx.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2efcasxjm.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2wfapcscj.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tytctutq.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2zxuvgyhw.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2uylowlxl.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2ugtebmgk.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2yofcmmyl.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2fpcetcau.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2cniyawqm.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2dnshutwv.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2cktpuuns.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2xjjztitb.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2mntnyanz.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2tbrvwjfq.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2fajnbryj.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2cwomedbd.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2vtlzwmuy.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2yzxxxzqg.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2abggeabg.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2azlqtadk.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2deauwdog.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2onhbmfoo.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2ppaigacr.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2wnlzuvnh.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2cykfstam.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2ipvwuksa.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2nkyhwill.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2puaynxbj.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2hgyqgibd.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2twlaopjw.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2nrsvdofw.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2rcnqfien.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2cdmpoygb.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2ardrteyz.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ksmydyzg.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2qcsrzrbn.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2riciaydz.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2zyaargqx.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2mijytcbv.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2phizactf.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2vqqlenyk.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2kbyncewn.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2nvxalmmz.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2jsgazzge.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2uwjmehih.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2phbxxhks.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2lpjnjbhm.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2jmidwkun.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2raglskrv.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2pxusydjy.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2grawuwej.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2dmijdgqk.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2zahjjtnf.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2ursriinx.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2nywtpdor.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2fgrvtnzn.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2lwtdgnhc.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xghdytzp.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2wsbnscye.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ndmcqpkk.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lainlsqp.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2zgjawqwc.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2dzlmrnmr.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2lgwipobe.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2svapzlon.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2xdxbbwxl.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2hthbcdtp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ygwjdplc.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2ebhztnrh.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2rddzzyug.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2uaiulsjy.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2qrzmihgy.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2dxhoazdd.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2xenmwvhi.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2xfcmdgxd.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2cyirwwcx.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2terzsxyq.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vvlqogpj.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2crktjigo.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2yxxvncct.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2tuhpfwcg.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2vvzdotqd.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2hlgacuen.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2sjnpwyji.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2rtmyljnu.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2xaxkbute.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2nyklrviw.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2oschtydq.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2covffwal.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2puiobuvk.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2zxadbjhc.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2awmnjius.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ehqtldzs.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2kcmaxtqt.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2zlitmhsb.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2sugpyegf.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2mfolkrlg.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2xmzbvzra.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2xpxazeuj.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2vzvdhivu.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2ievjaqpg.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2qwjptpol.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2bfavjqlu.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2vtkinqxv.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2uijvpozg.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2byecrgir.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2gypiromj.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2fzeijvlz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2pghndqnb.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2qosyjcsi.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2smurkpwu.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2evxyhzzj.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2thowlbrd.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2qnniehxz.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2nopngsqw.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2hdrkxbbw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2xmwblmxa.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2lnfmpris.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2rhygbwct.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hbdcmffk.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2ujefrvyz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yryudswg.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2kxzjlqjo.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2tcmxiayg.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2yocwciwi.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2egzbnsyy.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2rfvtojfh.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2qdpxujic.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2bamuwjfc.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2wcaooaat.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2nqrmiihp.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2nyrhpley.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2gbprheem.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2plvoizam.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2pcjtixsa.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2onxoqbxp.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2ggwvdfci.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2yqpbidri.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2xcuamhpm.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2ncyukvsn.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2yobdncny.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2myncvcjj.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2zbbuuryq.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2sdgdmrqy.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2fjyvgrot.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2psjcotwv.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2byiumcjd.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2lwdihezj.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2fleimrkh.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2dieccezi.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2zictabdb.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2bkgieymt.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qbxspapg.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2uwvipvyd.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2qufsygxm.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2kexsgwbe.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2jwynmcky.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2balhnksy.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2madeoexw.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2gxltbtsv.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2efhuyebo.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2raaysexi.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2lpdhvtjj.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2dulknkmb.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2odvxdcbd.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2dfmnrpgg.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2frphduwv.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2nznbmvxo.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2odjvwtdr.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2lqgeysen.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2hxkpzsow.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2occpvuou.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2stsifoeg.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2igimuhbc.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2livcxbhp.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2ltmemfsf.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2uvotszcn.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2yveyutcg.html


<!-- 参考信息 -->