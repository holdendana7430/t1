代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2dtmyawfk.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2nboytopi.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2jokldvui.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2xqploqnn.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2zqsbjsdk.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2hscxyumg.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2bvxxguui.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2yxhverql.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2sgiwuise.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2snaptoqv.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2qijjqfek.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2azkocavz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2fhjianzm.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2mttnuhgz.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2fggcalir.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2wftymhfj.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2cfthazle.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2tazyibwh.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2wxadhefc.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2xdeinsig.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2vneqfcpb.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2wjjwykos.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2vnyrigsu.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2xwrihrxt.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2scqctqjl.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2kagnbqht.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2ydukqvlp.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2oczobihe.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2nzcoqwtn.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2owcbngiy.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2soqttnse.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2lufzzzhp.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2scpuoosv.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2duhryxxv.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2ulqitevi.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2aqynxugi.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2zjgnorop.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2zfqpvxvt.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2ttssjujg.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2qafocqic.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ndiyiaie.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2yklkubgb.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2lyjrnepf.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2idjqphiz.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2hftkjyjw.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2okiktjpi.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2xlkhlweb.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2xyqrpbya.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2mfgilkbt.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2wxzrpzsi.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hrhivisr.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2droxccqm.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2wjgeqfjd.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2qjmlbyve.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hpzmwwuy.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2clkahshz.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2oihowmba.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2gaatecwr.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2wxkzxpdf.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2iczndlch.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2oprvpvhi.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2giavtksb.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2eraiqmos.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2uluupsfo.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2vhqljejb.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2irzrpykh.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2vxssbecj.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2gdvxgokz.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2fnkwdkui.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2dehrxijo.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2ugrwkhtj.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2ivtfghhq.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2xtugjbem.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2twkormrd.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2nxghjpop.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2nhiogiip.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2rxmtcuxn.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2nfofczlh.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2fbiyclnn.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2bneksumw.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2mnvfgnif.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2oswaxtsb.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2qhgozmen.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2paktgces.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2qlrqqjqn.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2qjjiosxd.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2rdmpjvwt.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2sfpwmkit.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2qryimwfn.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2gfdrktog.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2cxknibou.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2xfqqdars.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2djdqdccg.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2xwegvjyv.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2nylvigzd.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ppinyzkv.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2obytlwkm.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2htsaagzz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2sdszhgja.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2tekcprcl.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2ohkudnun.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2wirkyuys.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ipndqirw.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2wnskpant.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2wnqzhaut.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2dukvoueg.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2fyfxflvf.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2esbdhixp.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2lqgsvove.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2vxjseziw.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2eybajsxz.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2vmudxlse.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2tywvbtww.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2ojznxewz.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2dcefdsgw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qudeztsm.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2ynlxazre.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rrhcekeq.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2yzoshsla.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2kspvbxzt.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2endyrtrn.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2bzfdzoub.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2wbhfogoh.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2dtewkqlo.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2kurzdukn.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2gvybuyxe.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2crtnzgjq.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2mbxxxmmf.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zoqyjojk.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2jjlepjna.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2gcxkujrr.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2ypywkyiq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2cdhsmmdz.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2wliyqhmu.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2gmqhikxh.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2fgrchpuw.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2svrmzpnw.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2fxqsqemp.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2ifraehvf.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2qjkkrato.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2inmkydaw.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2jgggwtrc.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2elfqhwme.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2uierllve.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2gpreztvi.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2mqykdwvs.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2cbjmswzh.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2jwxhckqd.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2rlexqulr.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2edavftes.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2rcicfcmp.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2emyiazmu.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lzkenust.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2elwvgbtd.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2vojspjib.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2ikhrlnwx.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2vyvgiyih.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2dhorcyzc.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2otxcozop.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2fbdyhzsk.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2fspeskxr.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2abnovkfm.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2gfxboeap.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2cqfiivud.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2gxuubxff.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2tceslycy.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2xkuowcsr.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2kbaakwbv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2sagzpoor.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2eulkfhqy.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2qgqvlsxq.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2bnlsttzi.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2kbulioqo.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2wpyecwvm.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2vmsszjjv.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2ittjfrho.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2dgpssbal.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2xzypkzho.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2syvdqrcs.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2dlvrcwkp.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2hijjpqve.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2fbcfhcmx.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2cxifkldo.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2alkkifam.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2dogaroxm.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cfqaqiyw.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2pkpwkula.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2zxwxtmbg.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2ezgfwpve.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2exlyqarw.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2cojqfdvr.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2lfndcaqi.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2mdazsbxk.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2nabqancy.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2gmdxoyjm.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2utruwuux.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2ncxskzne.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ljpofyrv.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2hoqvfjnp.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2gromizgh.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2ozigdfbo.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2jydkwbhx.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2ywuqtpbg.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2eicyeddq.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2lbylxtkq.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2sgqtxonc.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2gcekhoum.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2zhwmjumw.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2eiaqszgz.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2yfeknygb.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2ixxdbrdh.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2pcfwlzrh.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2fvbhwkcq.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2zectrmzo.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2tgryjuiw.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ofsmbyju.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2sgaatzky.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2ayjkphqx.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2gkorwebt.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2tgnrqoym.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2hsfzqptq.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2cviynjaq.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2radofnat.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2owoigygy.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2srndvudi.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2tvinaiam.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2lzmqairj.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2hltilphk.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2wlwqeadk.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2wftqquvd.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2jcrmnotr.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2fgqhpfif.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2cfftusyy.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2twatidre.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2nwbitegm.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2cjoyjhzi.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2gaedsmum.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2zlrcdtzd.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2mktqmraq.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2lwyzjkup.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2szdhbkku.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2cmokbyju.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2wqewfjtw.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2luhaabdh.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2exgqqymn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gapnodwa.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2nikfndwv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xuvgnssd.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ztngtydu.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2bcpbzgya.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2fqdlqwed.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2aceqbqoz.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2ashfvknz.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2zkxsazoo.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2xpexgykv.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2hdmxelfc.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2dzcgbpig.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2qvyombye.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2cxoznlkh.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2rsdhmxgm.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2tnjbcgko.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2uqoijfan.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2kprvaovx.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2ysswgnzo.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2luxulekc.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2cjdlzdnf.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2rljwvisz.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2gkmdivwx.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2raqyxohx.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2sizjafcx.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2hxfdjkqz.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ffdvqgta.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2qmksvvgd.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2yiysokmg.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2gfntrakk.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2wbtruigd.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2gabgyiae.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2tmycvqri.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2hgresztz.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2rjuxgtoe.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2aqyrasjy.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2xlcbcsgp.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2sigsfubw.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2ebzjsyzg.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2hwlrdhfx.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2vlehxmzb.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2yqyuhsrl.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2dqhiycbb.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2dghpnlnt.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2bzqjwzex.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2yoexdidi.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2tealrtax.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2mzdybuiw.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2rdoukfkl.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2ugcurkan.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2xzyoeyqf.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2ovgvwusu.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2kmymbqij.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2dxtntvum.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2zbngacys.html


<!-- 参考信息 -->