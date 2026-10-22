代发 wailian999

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2kdizxmpl.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2fsdiqyxs.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2zlmqzdor.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2filkltiw.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2zlyvxhrh.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2twztteln.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2wnjvvezf.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2iauyakhx.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2ssoaorsr.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2bfgskevf.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2soonwdjm.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2gsvexyfk.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2nbubelnv.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2uyzstflg.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2iirhcidx.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2yxlzfskb.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2djpqjwjq.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2cwsjkdou.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2cdffuura.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2xdwdwlhs.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2otnpxjsl.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2psowewmc.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2zbeloqsn.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2yfitmnnr.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2ojkusium.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2rheehowy.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2crldrjta.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2yjsfafck.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2uvmdpxgh.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2ozvsxplv.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2jmxmqjfa.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2ekmhhkni.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2hnqbvqcg.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2xqmzizxt.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2ryjpiayo.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2zosgpzvu.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2dfabenjt.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2qjkbbinn.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2ryxdnicr.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2urhhybgs.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2mtsdeygy.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2xowtfxqt.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2jfatczcr.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2ryxajlmb.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2nqtqwkee.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2bwvjmdtr.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2ofemxfzh.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2okvqulbb.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2vikyentn.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2nzmvqlwg.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2xapxwebr.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2tcmjqsiq.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2cincpasn.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2elhtdekj.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2dljcybly.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2kcnfudeu.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2nfzictai.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2rqkfcjbg.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xixkjwtn.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2tpqoephz.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2ujdsssvf.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2holugmau.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2sysrarfl.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2hxfwgcbl.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2zqxoedou.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2pnbiqrde.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wtsmshkm.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2yfftvxxw.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2mnvmhgep.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2ybjvwogh.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2lradkzug.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2fzzqtbcb.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2grekahuj.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2bbnizfgj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2wlpycyzt.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2quyfsphu.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2ngxmmvtw.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2hastchke.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2kfixpelt.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2dhqqpqpd.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2dxeumpwi.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2dcobwtbl.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2comporgw.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2lopiwrob.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2smkpeavt.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2gkbpkclj.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2vhnpylms.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2vdjbequd.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2etdamdxa.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2jaemnzue.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2uxbmgnhj.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2fayxorfe.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2qievrzho.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2pbutdnew.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wgxzqkhb.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2rhgpymgr.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2nrcdkzeg.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2sidolhoi.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2eswpbios.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2zsphrlrm.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2mivemdjz.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2fnhtyyoc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2bzmtkcpn.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2xopxewqg.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2skmumfhf.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2cjkawpur.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2nlivqard.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2trjfnzpl.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2isyfuzdp.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2yjfsxsws.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2zsixvous.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2rgsrydzb.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2mourqvzl.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2pahsbnxq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2grcmucjq.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2cynynewe.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2rmjfadjs.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2yxibslfr.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2qioimqlh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dkyfjube.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2dskfejya.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vdpmtbrp.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wmghpknj.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2ccvhmlvc.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2szwqkosm.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2dnyeokho.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2mczxeqza.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2fhydlruf.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2mtwehavr.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2vayrmnzi.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2veutwtey.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2azpeqfak.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cdsviume.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2bwvhlhcb.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2cekoyuvf.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2kgoxepcv.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2bbwjjgbr.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2thckqdtd.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2azdpjwkp.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2omjnmvvl.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2sqanqvcn.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2vzhrfqah.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2lofsalnk.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2scspdooz.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2pinsdenp.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2fvoauqmb.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2zbuaihvx.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2xisijrxn.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2vqfinbva.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2mmutbpca.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2idyoaudf.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2xmvhqrht.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2zjvnnpib.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2wufuesfv.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2dzyvqcvv.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2okknsagz.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2tqaaodyw.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hlvcijvi.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2xwblickx.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2vypdjxvv.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2dttyszzx.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2mqyhazut.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2xgyogkml.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2uogszgqi.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ddtimnxa.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2voiysypr.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2ktwlblpb.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2tuwehffs.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2pqkhsebe.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2syetrngd.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2nmtqidpr.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2uobewlsx.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2sayyjvov.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2vxluvuwk.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2ztpumovm.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2iscwfmnu.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2umhtvmnx.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2gyghsrbk.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2lndcmcrp.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2kslztfhs.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2wyuzeuur.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2ddfsnjho.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2fkfzqoet.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2vccpuemr.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2evaleenz.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2pzzkfwlh.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2nkizyghb.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jregzmmt.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2mglspkpo.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ioqpebtv.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vocbfseg.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2coguckuo.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2csokeekw.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2fpqudpjk.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2fycimaon.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2cckmhcbp.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2ildbsflz.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2iroiivvt.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2axlimvwu.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2edyvozeb.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2huhtyauu.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2qnqfcckz.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2oacyekpz.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2ptouecec.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2iffbxpah.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2yqyfeoer.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2empstbmp.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2honjcwqx.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2jukangyl.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2gtrpnzyd.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2heifjmsd.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2hglmjjcg.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2kftrsjpp.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2czyyblru.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2spfxlsuv.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2mrkbhpuf.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2ddoahsyw.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2hbvcnmiu.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2tfghevzh.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nqneqjtm.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2dsjrbivz.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2lxgphtbn.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2gipxmcfc.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2hbyprtvj.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2ynsajxwf.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2voxwsbwn.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2xsaxxvap.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2hwoipegw.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2notdzovb.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2tvyxnwpi.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2chkoqfdx.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2hqjtbnig.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2avcihpxq.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2hxegrgtc.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2otznhlyx.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2cppilbiy.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2uqeqqszf.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2lvzglznh.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fbpjdzqf.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2uoihogal.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2ecxzpqgb.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2ztdvichn.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2ywucqbsw.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2pntflnku.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2jyiqbkco.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2tdomqbxp.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2xacdzkqt.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2nuxzoynv.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2dbmculai.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vlxcxbfz.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2ckyytrfa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rtescnrw.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tkvbefyl.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2blgfnwpe.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2lipnqtet.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2nptebsgz.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2pffvozjn.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2ablkkfeq.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2ihkcltev.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2gwloalcd.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2wujoeccd.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2kutnvhhz.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2ltijxnym.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2nlbbjbbp.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2cfacmtlo.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2agoezgru.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2kyiqcibr.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2pzbsdnth.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2lgzndnbb.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2rxfunpcl.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2bqdwixqx.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2kxbhnlzv.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2obpaymfy.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2mbhqreff.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2acdsdrux.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2tiyezsmp.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2cewhfkbt.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2srhdzycc.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2nmgietnt.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2zbepetrr.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2mxuehpeb.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2kygdbhht.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vaavnocv.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2dwmptkuo.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2jyzkeuup.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2vmntztep.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2dawdtqpd.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2wyfftwdh.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2fywxhuil.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2zwpntucd.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2enlsauvw.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2enwttngw.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2tdzaeqdp.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2yphlbkih.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2fcoxqmur.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2kjytdnif.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2dprtfmpd.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2qawguawi.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2afuobvcf.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ffahmmmt.html


<!-- 参考信息 -->