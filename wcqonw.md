代发 wailian999

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2fkbeogib.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2lqdvnzer.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2yyrqtygz.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2sdjgmbwk.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2ccjbtnfj.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2mrjhlwiv.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2ssbmvkwv.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2hlwnuaca.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2qzllxgsq.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2bmtnhjhy.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2tsqjusmv.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2ebloxowo.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2wwzejmiu.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2gehkedpj.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2hgovtfcx.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2wdykdzuc.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2aamducyw.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2maoibmrb.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2lhpgxgbd.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2cntqhkdv.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xtlooxxb.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2hhfvqvhv.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2sxrehfvh.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2homadwqf.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2uceerrkg.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2zzgjdfrx.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2hwxombma.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2qltpaieg.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2ypowumrj.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2rorbpavp.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2gtkhudqk.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2apauckwg.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2sfhuvxrr.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2xziyhwkd.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2hlllcpno.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2mzjsecwz.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2bnkvsgmn.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2dwwimacz.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2utrtrono.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2qkmkobay.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2vqpnagrq.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2qlbsgvem.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qpymkvvi.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2qgayrfln.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2arpgoxoy.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2xouqgezs.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2fvtntsbf.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2jslsjhbi.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2sdolnudb.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2hbhcjisi.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2edhzsmvf.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2fyfrenuo.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2qvbmxwlr.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2vbokxlog.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2uotvizlp.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2wocltpsp.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2pdpxuqsp.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2vchrrfuf.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ntdfbqou.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2ccwskpcl.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2fatjkuvq.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2tphjqnxx.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mxoaxzty.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2hivlwknr.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2xdeedhjk.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2thehtxxi.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2ebdvrpmi.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2dhhcoqau.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2vtnttuyu.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2qypnefwg.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2xbqmosox.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2yderhpnc.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2zukuzckm.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2olmutffm.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2xwwtoohj.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2kwuihhmf.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2mmblibdc.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2xrduoeyn.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2vooemcgu.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2sxgkmtbs.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2scsxhiiw.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2dqvbjrjh.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2etzohgww.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2sbzfrcta.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2blgnxxob.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2xwyownct.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2sffilsrd.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2qyrxhzlu.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2ywwuxebx.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2xrhmxnyr.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2gsusuvqb.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2sdpjpcta.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2wyvqblfc.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2nrbqzdwp.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2usxvsyag.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2hwpbtbwh.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2stwodyjk.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2sogwxuan.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2knghndid.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2qvmtjhkb.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2jgijcndk.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2xiwqeprz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2vdyzqlvb.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2rzmelflc.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2lzuypkmd.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2njyrdabp.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2piwfstza.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2qodtwudi.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2bkkepaqe.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2hoqsqhok.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2rghwwiok.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2aeavyhpx.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2fhwyerty.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2nbnwzntf.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2mdrtqawe.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2wijnjcfx.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2cljxbipx.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2wambtcay.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2twglvhpy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pxcsavje.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2kagdiowx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cfyczaqm.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2olfzzgzg.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2empdndsp.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2wzxpcqax.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2aepgctws.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2jwjchzsh.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2eeoaqxrr.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2lrhoasxd.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2pqjdcpzs.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2gcdjenrk.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2rzcgbseh.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ximfzjww.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2qxfnpnyn.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2panqhevb.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2rdcdrhxq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2mxorlyxv.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2ondomdnr.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2nueruokm.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2lhcuhhcp.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2rrloqbbt.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2ceongtpx.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2mztnfkjs.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2yeaekfjp.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2ltvedwfn.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2qjghblfs.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2bzysbcdv.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2dfzsveqj.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2wypgyacw.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2lzkkpftf.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2azijvxxg.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2dysyrdck.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2xqthdixm.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2ejyqatrt.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2dgpcihoe.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2jhgfxcce.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2lcsjsddw.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2tlqytvgg.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2xjhstqdk.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2qvnntvtq.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2apcxieiv.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2zuutswfc.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2bukxnsty.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2xwaxrlnp.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2nipbpnct.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2uqrtxaua.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2khadjmdd.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2olwjzcmy.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2eeafsvaf.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2uhdlomeg.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2siceboxf.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2fgsbpidh.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2gktwayei.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2kffvgpkg.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2aagyrvad.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2lbceygfq.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2syephwkx.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2rlklhppf.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2oqvxvycr.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2xvjiiqam.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2pbeoittj.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2obepghcx.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2gcqyyyhm.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2zgtmekwf.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2odrakzgu.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2mnuczyde.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2aclislzt.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2gipckqzf.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2wilwtksc.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2wwoxbykz.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zdaotqat.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2reylfxxt.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2egytpagy.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2sroaowzx.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2jhilxvba.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2oxzhqiff.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2iqfpxvvk.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2jigctrkn.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2zncmvzhe.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2uoxkrxxl.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2qysqhfkm.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2vzblpqxy.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2rgikdlzq.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ffyrbvuy.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2ojxzloic.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2tqymhmwi.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2ialvnxlo.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2hpilclrh.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2kwjiolxs.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2xdkxmvpy.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2jlgogxei.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2ywixcrhk.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2dkjyihaw.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2hzlommsp.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2picjipaq.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2koopvwbo.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2krrscqzm.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2seewrouu.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2nlshisil.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2ilzcqjsk.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2gddgkqkf.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2tubfkgfl.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2tljhfkzu.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2vjlvkbkp.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2zwpcumju.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2fidqdxqd.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2cddfkgup.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2dguxoqke.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2yttddfpq.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2mdwxgssu.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2hzblgmrm.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2zqgstwyd.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2idxgqaqe.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2zilgssac.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2aqvcjpev.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2qxpctzra.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2ffqfjqsb.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2moejsgxm.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hvrhskfh.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2tubiaear.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2lyntrtbj.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2bjplwyjo.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2kidxkgyd.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2csusmsrl.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2hufdxpfa.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2hcztqjew.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2wcqoxcdm.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2wyvndfnh.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2zquunixd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uetswewg.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2qvgzbyyf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dkpxurat.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jnekzngh.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2cxyqehhx.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2njzumscu.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2uyxvshus.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2yqmcttpe.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2nklpeyri.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2elyhntvq.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2pmhjnttg.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2gcuuxiuj.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2vhshukcj.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2rjckznrp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2cavgbrid.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ytjsxwuy.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2dienxizg.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2eeapgeek.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2butxjbkl.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2rfyzuiqj.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2ydxpvvmi.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2euxtqlcc.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2ksecxwfc.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2wqdgnewm.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2wxlxrozl.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2ngkwsuyk.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dfynwcwj.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2afnhfobg.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2cipbaegu.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2dtszzhyg.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2wrhumgjo.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2xmakhgro.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2zcofgrdx.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ywqviean.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2kuwzzupo.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2swuvcabg.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2xbpeabtp.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2pasyeuvu.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2hnkxdeai.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2ntgjmrbk.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2dcsswdkf.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2nsrfzxsi.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2eqfxrbyr.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jlkbgzjm.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2sstiwthh.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2cqrxeseh.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2jtnjiupn.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2jzoyzggc.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2jsuarpkn.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2cljgxjkd.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2jmoccqbw.html


<!-- 参考信息 -->