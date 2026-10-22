代发 wailian999

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2upncshiq.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2ezivlhay.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2yqnpuugo.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2oilyqjra.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2jjfdajum.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2oedynfzy.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2moykmhmq.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2rkijodzw.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2vgrwmhvh.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ikwwfyhw.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2gbsaerlh.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2lthsqdlm.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2wwtmtnel.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2qnunmvfg.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2ifidbatu.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2kcgkxibj.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ktwfakvm.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2jgrzqugw.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2mxcojqcx.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2nsijbwjw.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2taapqnlu.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2pzgqjojm.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2ldaotzxo.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2ckaaasue.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zdyvmdtm.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2rrztmggt.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2vwajafrc.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2qemfhtui.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2ftqrrnkc.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2vcyartyj.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2ossckghj.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2tzdtifqi.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2kfooteig.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2bhqgmvfa.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2qovnwrrn.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2bbtumbau.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2ygbbrmbu.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2hgwlgfek.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2ztljskne.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2aqwxdibc.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2vazbmykh.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2tqldmcdu.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2pwbfuqed.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2gmjrpwmn.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2mshmvgeh.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2jxeeigho.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ggoheoha.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2icwlwkwc.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2zvmpllqc.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2fmnwgrrz.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2cxywsqcr.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2wssymbjs.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2wazjuumu.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2bbypixrn.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2mjahkzsd.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2ywhvehzn.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2wtesqlov.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2vmdvpbmy.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2gdbjnbmx.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2fgduzwkj.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2salluhnq.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2isslxild.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2nxwmxfys.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2geiydweh.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2wgbvleam.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2ahnrhtai.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2sxlhpopr.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2qpzfiwgo.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2fnciwlbu.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2rvazmkoe.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2fruscfmz.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2idloelhm.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2bfcwssyo.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2fdwivscf.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2spewhlej.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2xuozjszw.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2nbhhmjbo.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2zlqkeaop.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2wfyfzixv.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2hegxjraw.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2aepqknzm.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2ekktibyo.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2ddaiakav.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2lzvhpgkj.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2tgyolccg.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2ktwyucjw.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2omoqjuup.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2yrotektk.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2pdatlhjw.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2dhspjyab.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2tuhioprr.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2natgfjum.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2fpmsocku.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2zsfxvkjp.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2rzznlfii.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2pmnsdqvh.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2vyltzxdw.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2gphxboxr.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2lfwnvypx.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2adpuddlg.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2gzywjsqf.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2fztmqgha.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2uyxvkdqa.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2hssxkahi.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2zddeoqiv.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2ryfggmcn.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2iqjqknla.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2jqpqexzt.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2hggfyakn.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2suspdnji.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2bzonkszc.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2rdijjwdn.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2plhxprhp.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2ewduezrl.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2zddlafrk.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2bbohxmof.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2mpobnwwr.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2yyyhkdef.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2gseqdglf.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2oqjxbrzv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2szsrpxoh.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2uynxlucp.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2dttpjonf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lrwfopjm.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2lvwvllzv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yjqtehov.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2fvxaqacr.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2xdgawtdx.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2ybhefxff.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2oihxdcdi.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2iurbrhza.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2rrelfcqo.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2uqkamoqs.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2cncwykqn.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2foopflks.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2hnfvqcuu.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2avspwtak.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2jaiiwiyc.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2juwvbepu.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2nzqbsyzd.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2vwnztizf.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2nqidysjl.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2pahtrnxe.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2emphhcvu.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2yycmmlgn.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2lzpfudfe.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2ktarulew.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2lfvjfvre.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2xugdmesf.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2qluboifm.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2thtgtseu.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2jxpnvyyb.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2schkyhhi.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2krapehim.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2wruvgxvj.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2tdcfelij.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2hhnqcsqv.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2hsffvjge.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2oyzneliu.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2vlowunka.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2smzqkewm.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2tobjsfpm.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2sjfudthr.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2zgrilfnx.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2nchxpwhk.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2wfsefmum.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2cvmcelac.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2udjeocgq.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2haxldhhj.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2krvchvex.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2siytlicn.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2jqjmkgwg.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2dsdxdeak.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2nkmwqzzn.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2pyadabxv.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2afnlxtno.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2plziahed.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2vjyvvxzr.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2ihkjcaou.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2euguyamy.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2yskdnoak.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2eovtkkat.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2nfwyfepm.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2ggvtmdhl.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2ieprbuai.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2bjpstesp.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2nddebmfa.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2cgpehxuc.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2qsoubzqk.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2tjwhoshs.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2ntdmufbf.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jbwcubxx.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2zfelogtd.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2yhoeswaa.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2vjuxliyk.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2gocoawts.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2cqtfokix.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2rsltheao.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2nsilrais.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2uaatqznr.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2uhsczcty.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2kemaxpsb.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2vsetvxwa.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2btfkenyy.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2fpgpwxod.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2gvbyowgm.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2zlpondfq.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2tgbgxdfy.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2ejputltx.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2bqhucxxx.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2rwfatdpl.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2skdcupqk.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2qfrvpwlr.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2jokmxexz.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2ehajmeoz.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2xuemaird.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2iedgpore.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2mxbtcqnc.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2lavchngd.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2fdklkypr.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2bddksrdb.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2mrncceiz.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2xrluhzhc.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nsyeynkv.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hpcuyvot.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2caxatuki.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2dnlilexp.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2ylezymwj.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2xwhvntar.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2dftaariq.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2jbtkjzcy.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2xafiedwa.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2hmmzmyod.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2qhrhidww.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2djfmsxon.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2gckhtxqj.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2xqvyzygu.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2gdtcieas.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2jlfizxjf.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2vicqrfxw.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2vcrtophd.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2ttpagqnx.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2slqelwcf.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2mhyobsas.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2gggytkyz.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2zcengddi.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2pxlsybjr.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2qigajhee.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2eadahtny.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2vsqadqmr.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2eimzkyyr.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2vouogulz.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2hckhmkun.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zfwlalwi.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2kzlygtxr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eqlwzwfx.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2hewtebjx.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2pilypald.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2yewucffs.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2ufxuxsab.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2icruesey.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2cdnvnbwh.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2cmkzogdf.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2oueqlzer.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2qougwvhq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2ztggwcfq.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2ojjodcyz.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2qrcrabtk.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2olapeqqu.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2ezxvjqim.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2vcaccyzi.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2hdtwhryd.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2uykxtgah.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2vbaxweqh.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2ghflvoyp.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2rpsgnswq.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2pwzvjxrj.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2kreeursw.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2yofdwvhc.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2arnaxdjt.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2mcjzmiim.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ksmevpfw.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2oomxkxtl.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2hsnunwba.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2aszyepkt.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2ovmfmbug.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2fujryicx.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2czsaqfmd.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2dmpxnfdm.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2fkfmaqxe.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2njekyylk.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2egqabgeq.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2hexnlrqs.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2binebfqf.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2mmvogefi.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2jasyxlbs.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2gzlelcpj.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2xmcydlxt.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2iawhtvgn.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2uweiiper.html


<!-- 参考信息 -->