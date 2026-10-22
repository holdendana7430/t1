代发 wailian999

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2uxguahjs.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2vlbmfzrm.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2ulqfdgsh.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2ialjxrik.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2gsgutqmq.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2qoznvhhg.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2dlkiovfy.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2yjvownjv.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2bbftyxxs.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2zobteppo.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2ymdwmlxp.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2rtgbhtfu.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2diuzzodm.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2tgrtioul.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2looktmma.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2qlzwdvyi.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2adtbssqc.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2buqaobfw.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2bbfkpdin.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2sesjdjrf.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2zjbguvfy.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2fcaaeppr.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2mrquyhde.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2rqaopdqr.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2hssswfrm.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2whipfvhc.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2ieweiozb.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2vxoagtht.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2vajgbtja.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2nvynoppq.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2itlawmmq.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2bhohfdxs.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2jherwcyp.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2osmuerfe.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2cndsrfce.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2eqvedjlm.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2rjvcqwrz.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2kdivxygg.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2jmoxcftg.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2ywolhebm.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2satwonek.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2yeizbwah.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2dmacligr.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2mvtxemoe.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2swsyjkni.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2juvkdeea.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2hnppkrgu.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2qvdfmqkm.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2tkqqqixh.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2ydahwufh.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2noyfelty.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2qvbkpjyv.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jqznohqr.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2qawoofmj.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2xfbkznog.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2snptbqbe.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2rqiazitv.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2umigglrb.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2vebzppnq.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2lszvtgcr.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2gzxaplyw.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2vtuorwmd.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2rriagwhk.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2dvaomklz.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2trlhpyuh.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2nwqwagrq.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2cpwzodhk.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2usmcicly.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2xcbjaxhe.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2yjyjnltw.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2gxrcsrkm.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2wjwqxgvf.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2ryukgfzs.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2sqesbkso.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2ynzrvtrc.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2blbybpbx.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2rchdtgjo.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2svsfwvqw.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2jrwobagi.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2vfntngvx.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2gxqicjbv.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2ajjtqzlg.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2arcgaoay.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2yyhpqkoo.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2erkojqsk.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2nwrmngjf.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2yschqpet.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2vlanjtcx.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2gqkrsfeu.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2bhdwgzkl.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2tzzmvcwa.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2ifxgkynn.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2uwfdmdxz.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2rdxbypat.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2gvpiihov.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2paddfecv.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2oeldmeeh.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2aydictgy.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2ammbzddi.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2qrsdyggh.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2ltowuunw.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2xsrrzxqc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2uesgdrop.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2rywwtjzs.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2nnumjzzb.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2uonvobbh.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2fnqosiad.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2lclvubkc.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2gmusomve.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2rudbvzdc.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2kgjkqjog.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2zoasrkgz.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2sinzcsbl.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2qggtrhpk.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2zkptzipo.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2jkykdgkz.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2kabbmnzh.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2vwkbgigt.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2xccpicvb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zikdfyvj.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2xmikevsr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rprzhkgq.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2mreuimcg.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2nkmmcgfs.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2zgiigmlo.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2wxxxdsph.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2omcrrymi.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2oapjjmwo.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2frpwrkfa.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2dbjstcpj.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2tocpjrpz.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2sayuaita.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2gxxsxvve.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2nqevnvsh.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2idxheqbv.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2jcqhhtbc.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2porahjnb.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2zfmwflef.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2jkzwsqpw.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2mhmgmsye.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2svahrhvt.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2qmtbohhj.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2xncwahxa.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2nydihllv.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2mxmvnonj.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2heruutwq.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2nfdqxwgg.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2jgrpxwyc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2szhlegrs.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2vevqoelt.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2opubnjdt.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2wugvhyyb.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2wiyfaspd.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2pyceddjq.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2lfksbpwh.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2muhbnvhx.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wjgnsymn.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2osovwrro.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2gaeeemtg.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2jgremglm.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2mbosjzzh.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2smtlgcjj.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ffdvzrss.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2aazqjedb.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2erbzlxyw.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2mkxpwbqg.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2ieoapgaj.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2dlecvyvg.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2eiwbxmds.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2aliubxdm.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2muqbyuvd.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2uewfozru.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2zgjvfyne.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2dolxoyda.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2lnlrjmzn.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2xyeqzzrd.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2qsqwpzvv.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2tfkojtvt.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2bkgtuclk.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2ilgnyump.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2gsjotygv.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2cqilhjuv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2nayfezzy.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2hmqfetqf.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2vewkwtlw.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2equyibyw.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2qilabtpw.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rozoeqyw.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2ofvwpkaq.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pkuwicvb.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fzgjaqod.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2axyheqej.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2uhlplquk.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2tqmddmtx.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2nzmmbdkx.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2gwizcrlf.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2aiisuapp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2hdrmdwdw.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2pfofhtqv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2khvropgw.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2bycsrkww.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2qnekbbev.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2dlbwjjmx.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2encyotul.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2bcikwxfn.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2uftmsynk.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2uqjeaulj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vrbekcut.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2rekohuae.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2cwlnwzdt.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2ryjefdzr.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2tbqyjvir.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2pdcjlufv.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2olkkyrpv.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2lgmsbevz.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2uuejkqes.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2hejcqrjt.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2dmzybnpa.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2xccyevww.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2wynwkesr.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2vehvosuo.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2iudqgprt.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2yzmzmqds.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2beltqylf.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2buofczly.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2cfaazxju.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2bjjsynqn.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2tpgilyzn.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2rwtbafsi.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2gvfuvktw.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2nfmtgfpo.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2yxierjke.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2vtvlymkd.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2pfjhpgux.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2fxuavtbj.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2irnmaqyt.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2yjspergk.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2xojtitay.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2biqnblag.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2zprgesow.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2bnyzsdki.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2yqwkjsnx.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2phexdtil.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2qutbdoat.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2qffomzij.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2hiyvnsvy.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2ydtppsia.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2ijmpmnrb.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2kdvbzvdx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2upngnink.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2sfxebrdu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2whxuwoup.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2oghwnyij.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ybhjalys.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2nofdckfi.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2geddhthl.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2icgndwtf.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2sewqvmpb.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2vxagvbfl.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2dszimsqq.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2dcgqqxyj.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2ogjykezm.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2ywecbhvr.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2xaeqernr.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2jrrmhqci.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2ccyimhzh.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2hzqttppe.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2yhhjlccd.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2cvzpocye.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2phcbzctq.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2ylczgggy.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2ieypopqj.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2rnixagkq.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2bfvdrhms.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2zdskhvcd.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2iuxpkxzd.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2qzpfomes.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2sdxaaljx.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2pubnljeq.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2jqnfkimb.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2kbsotjts.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2ntkucdrg.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ykkmdhxl.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2jmxmwihi.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2lmsvdrds.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2cdeoeseo.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2lgbajase.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2mjbixrny.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2ruoujkmt.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2htcinejt.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2hoircryt.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2soemsxnd.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2hazedtdg.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2ayxgsmgd.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2jhlsgvir.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2oloihsio.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2inaxqcbd.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2rwcdjfpw.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2gaofhfmn.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2mcruxzcc.html


<!-- 参考信息 -->