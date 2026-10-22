代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2inlnhikj.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2cqfeaxfa.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2nsxfopva.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2asootvfy.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2ynckuumr.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2lopbsbtl.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2lvlxuaoj.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2kgujoqcv.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2tinyusfk.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2ywcawlrm.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2hjnjkqyv.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2pgzqeijt.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2pwlqlnsz.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2jgrwlsag.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2mjzdxzdf.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2kccxjair.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zpustpom.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2yykjpotj.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ynltxigh.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2zrvmpkbj.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2cuvvlgkn.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2eegqmhrn.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2pevhnwxx.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2qbltimru.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2prjofoxn.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2pubeundp.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2bwgzxjsg.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2jnxzhwya.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2nbybtmfb.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2jeyqpfsc.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2lzxpzpmm.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2zowiqsgr.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2durdgkvc.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2fsvjgbur.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2zgnkksrj.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2kyvfxdxl.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2vwiclrkr.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2gedwvqpz.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2huenpfyq.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2oucfnusz.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2wlecofpi.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2rinzctwv.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2qrwyopsg.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2gdfrklwq.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2egvjrjck.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2ayztkhuf.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2itbhyzcj.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2qzlnaaeh.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tvgvuddx.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2jkdrrayi.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2oiwdzscu.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2zuddvfug.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2ylsfncrn.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2bznyalkq.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2xkpytoki.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2xrvsypwr.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2ywmeszgb.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2iqtajxjf.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2kvpudgmm.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2hxwnsdvs.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2giqaolnk.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2csgepwru.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vtacnhsf.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2nrsmkmbb.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2ueqauqho.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2zkcfpxxp.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2bmjzxfrm.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2hocagwiy.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2miqhcgnd.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2pujekidk.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2yelxfbru.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2krumvani.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2vwpjeagc.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2fhbtsgqb.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2dsqvzlzn.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2yxuyoqdo.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2icycfoew.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2rusabnao.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2fsblsbbd.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2tgavyhqn.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2vvkwdaze.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2lmstmndv.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2kgghmxez.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2yixkkclw.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2quldhoij.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2bzskzjbe.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2mtkuwtqn.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2psmgpdig.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2qrutdrkh.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2xvkgorsf.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gspkijol.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2opyojqts.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2tcpkaffa.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2revqzeln.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2eyhhiyyz.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2keutbydw.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2vstovkic.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2lxebxmix.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2quzfszzn.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2zzzqnzig.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2dtvztbzt.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2zjyxqshs.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2ihorbmvx.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2yzlzawme.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2tbmsskke.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2cbipepft.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2ajpbuakw.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2nluzeisd.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2cxeyysij.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2ydmecont.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2zfsacgok.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2euthwjpj.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2jxrvjhbc.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2wvdxwhok.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2cwzrlguk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rehqxyib.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2dbhgkdwp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qocnyghw.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ylxztyra.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2bnxxmpcr.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2iafmtbqb.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2puhsugjw.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2ydbkrsfy.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2spjffful.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2sjnbmrex.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2jogumxbu.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2vhzlzcce.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2pubxbchb.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nwopphas.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2xltspugm.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2zczncsdk.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2rihskfac.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2bjntsrst.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2ddfcslft.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2iacbqiwj.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2hvdsnwfs.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2vwkljzlc.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2fnnghqpz.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2grmyseze.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2qnchckci.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2pdxdanyy.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2xmubooju.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2ojuysovx.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2kygrwhhw.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2blgjgart.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2txqznuhr.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2inzqswpe.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2smtlsgbn.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2glprhegs.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2xnspshsc.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2hxftbqxs.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2mcszxkdw.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2avmitfld.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tqtnvovc.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2aiwgflfw.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2vxsxtkwq.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2auptxpyq.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2xvgjfsmk.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2elpbhmgc.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2qgveidwh.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2faxmexze.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2xktwldqw.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2qeaaoths.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2seqxrzyr.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2vkltzfyf.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2vyktkfrv.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2jsjtnhon.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2dmqpjmrh.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2xkhenoyj.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2qfimiued.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2euddiyys.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2ajrlnpmk.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2yrvzfcac.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2teokdlqy.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2pqtpfest.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2ryicevvj.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2vtqbynfe.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2ezhgsknf.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2tgfvhyuy.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2dxalovfu.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2yongzyaj.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2yetrnstu.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2smpkmfbr.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2pawpcpoa.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2igyzxeum.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2szyiaphz.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2pkldgwwi.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2pnvugske.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2ucvehjck.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ygszrgby.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2bymwxzcb.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2zykcdrrs.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2cqfkqorh.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2mauyptvw.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2qlmawdux.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2quniewdc.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2uruhorwi.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2mnxgeqor.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2fstpnutj.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2csdaedcp.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2gcvoxvqq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2rrsgjaav.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2nnyahgwe.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2gczcxcst.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2eyqxwdpl.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2njdyvpxk.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2jllxbbav.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2sjpabmrn.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2dxybywxr.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2ttodaoow.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2jsqxcvbs.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2hgmgchhu.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2cjfgbzpi.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2wiwqcxuu.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2hjhipkop.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2eekjyhqa.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2nmeqcogr.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2fjxyqwyn.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2gqaabvqz.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2ghytzycg.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2icaregdu.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2nqrkjikt.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2ifysrbax.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2zlcfupfl.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2pihwiumy.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2wibnvfqs.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2qfusrddg.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2aqeeqeao.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2bbqgnvgz.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2zecuuqse.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2tfibxfhj.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2blqqlmdn.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2jwztvyhb.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2sekqvbtk.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xouxyoer.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2vrumgfhi.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2lruhgngk.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2kzjtbgtd.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2iyrdmkyq.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2zfxzrltt.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2oyvcsskp.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2sfegrgid.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2xgvdynpp.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2lmmvezkq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2tbqiwerc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hsfnpfea.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2ywoyqvdm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xutuqsvt.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wzdlbhcx.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2axrntmxo.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2mfvbzjvg.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2hdodhdxo.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2imrtpjsh.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2webztzxf.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2zdwwpfdq.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2udjdmnmq.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2shptnjev.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2nfxkcrkx.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2behgiemq.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2mvzrzkde.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2anajyrfi.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2jkxhnsil.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2srhtdtdd.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2ovdzfuuw.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2ouhtqucu.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2uyhjnler.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2fmfrholj.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2dckeqhwa.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2peqbmbfm.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2ejmvpijp.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2ukrmjzso.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2woopgmxm.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2flmshntn.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2wmjhhuhl.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2emalhvpl.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2pfrrguox.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2mhppruqt.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2szkjdkmb.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ezaieiwt.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2khrjzsji.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2tsyjtmmd.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2speqqtjx.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2jjakkfxn.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2mdchtupb.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2oyqqdlfo.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2agbkqbwh.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2vmrulims.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2cvpmcxea.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2uhlvcvdi.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2ejfgsloy.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2lucxlkzo.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2dxhatnvm.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2wreouyob.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2irycknhk.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2ksbzpdek.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2mistbntb.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2ncgdract.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2omfirkmd.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2kqaxyiye.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2boknzrje.html


<!-- 参考信息 -->