代发 wailian999

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2esiswjko.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2xtrrtuyy.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2sqmyunff.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2xnhmldqn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2bmemcwsf.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2vxbvoepr.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2zoyfhmiw.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2hwdbzgra.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2dmnidnay.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2wdalivhc.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2sxyjvygm.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2fgmasiok.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2dvttozao.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2xwdeweai.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2oaszvxxb.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2cxtfbtlt.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2tidihvze.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2gadlghts.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2mkelywqq.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2yypxhblq.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2ldgbiksf.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2kzrjzuhk.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2lepgnodf.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2cuxshxyf.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2xirdushc.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2jshkhavg.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2cvjyermq.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2yhtgchne.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2xvtwlxxp.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2ssdxgnpg.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2xqupfpga.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2outkpgzv.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2cqlqjvsm.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2jqemvkim.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2lvzystta.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2xwxtigap.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2izmeiuel.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2xatrfgmo.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2kowfrbkz.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2bhplbgjb.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2qoxsgmkx.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2tgvotaxj.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2oevvzhmk.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2saelymzk.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2aogbunod.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2knncsrhc.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2xacqdela.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2tbngvitx.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2qvqajfea.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2duvcwchi.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2vaehwdbg.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2phizgnxi.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2hhpoxqzs.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2ziqqhknv.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2owubgvmx.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2cnbcamuf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2wrbtgemm.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2vvopxrfa.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2cylfeizs.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2nsqhdgnq.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2yczktjcw.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2czwozhjl.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2hgxhexyy.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2ifrdmpmv.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2sevfckjf.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2kvxrxoiw.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hinjjnol.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2ccpzdnvp.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2wytgoier.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2swtxghgq.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2yytudgoi.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2befodgum.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2tobpfjyn.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2bmlvpyjd.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2alvkeaix.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2xyjxxepm.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2grezmarx.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2csesdvrr.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2gljjotcu.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2uwbjjhed.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2mziyzmmz.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2okfrkkty.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2iaugjfgr.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2iuoqcxwb.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2adlwzqhi.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2fsucruie.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2rmwvfroy.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2iduhbibz.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2ayzukqxw.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2rhcgfawl.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2crkrbcgw.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2rvrwhiqa.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2cirrqrib.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2iobleczs.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ntdvlvea.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2xlfvbcuf.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2fdcfyuky.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2jllyeqnl.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2hdgnpsth.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2nurxbugn.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2nxwfopvs.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2nacouuqj.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2qcmjutbt.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2hlmqlgfy.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2skjrqusb.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2vvsalpbj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2lnsbsvhj.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2hmdguqve.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2mumpkttf.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2evkuwnvf.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2sjtbspix.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2ayqukcoc.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2inocmtvj.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2dmwodcwp.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2bhqlleco.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2zickqtfk.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2zhbwcvfy.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2jpgivhwm.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2wrfnfxgp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xyeaqffl.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2kpzpufur.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jozvhncy.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tbdaxcoa.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2zwwqwhad.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2vqojndjb.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2bmwzizve.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2aibvshop.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2wfrcqldv.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2nzppvhyc.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2enzfmeww.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2mhzoovfw.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2mzybsolw.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2tpshwngt.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2lgouzcxz.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2rsafangp.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2eugzsphk.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2hapiyxud.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2drtijurd.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2akvfcssu.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2ccvfvbhj.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2whjmzvai.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2shrszyfh.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2kfjizivu.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2qkacfaru.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2webwxoyd.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2lwmgdhsl.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2hzaadamz.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2yazvsmfl.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2zviowrhw.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2cuaxfbrl.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2rqvronyv.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2uxiekudy.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2aifhovlx.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2ykfrkjaq.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2qjorwhmm.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2ggticumt.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rxlhzbvi.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qbtjhzwr.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2dxvlkdug.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2aygfpnzz.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2xaidtlgh.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2opwoicep.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2grmmeixu.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2qhjurfne.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2mxyxlaux.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2vxfbisav.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2epdefppf.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2bvpfaqyo.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2ackmtxdi.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2wgkjcace.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2itdrkwrh.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2radosdbn.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2nkmaxeid.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2fswxorqx.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2tonnugpo.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2empitjpi.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2pxdnyqhh.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2eminvcaq.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2zmcaqzne.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2yotenwiq.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2tkncxkzc.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2nfjemyxl.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2pcgqrtwy.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2vkrejdus.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2rdplopbn.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2qddnjisu.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2hdzequky.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2cnjstmle.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2hjuatqub.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2cudbgbtf.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2xacmkmcc.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2gzapnimy.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2tefgdgyu.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2zzsgtcem.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2mxqfguce.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2xuvrfidr.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2fcunswry.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2bbrxrmtl.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2pclbkfec.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2likcaauy.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2zgkwcyfo.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2pcdwklte.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2fjkwuhfo.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2rdqgeqwq.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2lmxmwchq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2tohafdsy.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2hfszwthk.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2ewhjjwzl.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2npmqsjcp.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2ehxazkyl.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2emxsxvhm.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2xwnnwnce.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2tormzdde.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2cqaoykjv.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2imotcgvq.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2lqhvuksv.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2osfcbnut.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2ozcrhoae.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2mljekmep.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2mfijtijy.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2acytjfre.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2ezkolqbp.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2dykzjkfq.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2colbbczo.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2eenjglks.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2xgucwlop.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2bqprptym.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2wcyllqjd.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2yfhyjxnj.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2ctnsrtve.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2rmdloska.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2zuhcxgrh.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2kabdwfeh.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2aozoxzgv.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2hufajhcm.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2epnajxwe.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2xhsotcga.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2ztdceqfm.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rivqzsmt.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2xkkgalqa.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2ofruinxj.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2wibgdajp.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2nadczpza.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2jahcnpmq.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2yqcgwjod.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2asjtwxud.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2cpkykhhp.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2jifozvro.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2agowlfyv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eqxpmggv.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2zbkvtgiy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sbmqrvhi.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2pcfdyzue.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2gxtevjcu.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2thgturdk.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2xisbzeqk.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2dfwsbowr.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2eiapyvlc.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2dzelbvte.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2pqxpxlhd.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2ctmoqmol.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2dmkogixh.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2yzfllwya.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2qrsnuvin.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2pzalpuur.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2ydinojmn.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2lqsdmotw.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2rmrvfpib.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2qoqdsukd.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2jltdohdz.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2oxxodrjk.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2yldryngh.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2hpmbqeva.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2bjmrnzrw.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2shzzukyn.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xtdjitue.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2wekctgnp.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2yztgpgfp.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2gietghwq.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2wyrafzdv.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2bfnikmlw.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2ofnyqkiy.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2sxlwxddl.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2rkigipjp.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2iiwdudgy.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2wqxlnaov.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2doribhxl.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2ctlyfcbh.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2fpmsozys.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2pyfihdhf.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2xkyccdnd.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2lqsznnfm.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kuupvacs.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2shcuplci.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2hutleexr.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2gqgvnagw.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2jvkgnnbe.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2awsovwie.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2kxfehhla.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2wcvuehei.html


<!-- 参考信息 -->