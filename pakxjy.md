代发 wailian999

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3hxqkdmnc.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3xgtrdlnm.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3pqdlnelp.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3xankxhow.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3cacjomwn.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3oakxidrj.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3dczofmqo.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3qmzxggfl.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3qotqcmbw.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3eilagwvn.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3sfurbqzl.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3zylrjuoy.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3ejbjejus.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3rghaqcyy.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3lnbsgfuv.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3jumclbsk.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3kuoxrgbm.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3ccmgssxw.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3ysaiioiv.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3rryjwuyy.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kjoowsbz.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3hymgvhru.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3iutvqcwm.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3ezkxlghu.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3qrwfitci.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3dynhnsix.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3edhufrxo.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3bafjlilx.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3nimnpfft.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3txfmzwdm.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3wdchnqqb.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3rcqxryzx.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3vdcosboe.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3xumvmetp.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3ntmunlfu.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3zjfluocz.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3udvwabcs.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3jttrxcgl.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3syqtclgs.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3eirbvkvr.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3trfnoleq.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3pvgblrph.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qifexsce.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3ifgyqxoj.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3rbtnmgjp.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3agmmifur.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3spdvhahv.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3bnmbzkmf.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3lvyeckqm.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3bffsuhhu.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3tlveacvo.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3fiwsudws.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3uqlrfhrc.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3qiguwspj.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3xkvcqhtt.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3lehpqouo.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3alibvnbb.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3lxzhfuec.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3imeisrxm.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3ppstijps.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3jfylbrek.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3tbmjzpwu.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ajhyeqpi.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3ownbuhdt.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3zdojovak.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3xngmqeee.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ofabaany.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3hwjszkys.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3ftzchlfg.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3nhwbtcsp.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3crtnvvbh.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3ytrrbtml.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3spnfhdab.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3tdygbrep.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3pyglraqa.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3dfzxywhu.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3fsbeblcp.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3pykfotub.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3slwdutzi.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3rokzmxyx.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3decyyler.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3ohmcipid.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3vvgyojrg.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3jbkuezfx.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3adafdmab.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3lvyiuppm.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3jgdzryuf.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3uwafkypi.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3yardtqzk.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3ofhkiuks.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3vbnnbruz.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3zydiqciq.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3wvsolprm.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3yparrkrk.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fcdrnfzy.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3bzrbxtgn.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3ailjftct.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3gltlmahi.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3upekupoy.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3lrbpbhnv.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3qeutxeot.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3rxkiywey.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3bsqlkgls.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3hcwlbvey.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3gkyisobn.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3vjrrslyw.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3jbpbglhk.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3sbbpktlx.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3ijnaxhns.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3remchfuh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3joaezqbo.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3nreqhqpp.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3bxzofrhm.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3rjdbgbvi.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3bvxfwzrs.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3awqaflqy.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3kljvgdho.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3hxpfnjje.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3htuugoox.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3movccccg.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3ohhogmcr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3elnecldp.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3djqjtnps.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3jsqrieps.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3phytybay.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3gvptqmbn.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3ilnaluao.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3nviwyamp.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3jewuhzrk.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3msnffymi.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3mqfbyihs.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3swaaoloz.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mnbupvlm.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3zkrvivdg.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3duvftjui.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3ovrvqopq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3oqrvvsdl.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3nbmfunky.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3irayisnd.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3gmkabzwt.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3aijxitqq.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3qzblucdx.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3otoerblw.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3nsytnvpm.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3ewalgrjr.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3euucwgno.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3uvbxtvfe.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3rqtitsvr.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3xkwehxsg.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3fsrozogl.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3qokzzadr.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3jtxqusgl.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3uwaqyzss.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3wyarsdyc.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3amfiqfwg.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3kcitdtlo.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3yocppghp.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3muhnuvxu.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3svdzhxfy.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3lbbiavtm.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3dephzywn.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3fstllmtx.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3egszyyol.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3inqefzmw.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3znxpaokf.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3dsyfzjar.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3vfeigfap.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3thdupxqd.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3hdqoqkiw.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3jxppciso.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3foirczwr.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3bdqijhhb.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3svzetucm.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3sphvpryz.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3objjzkqw.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3qvvxzrcn.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3hxjozhbw.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3lrcflnef.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3cvymnrkz.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3xqxmzpxx.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3ylxsstos.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3nmhlkkvc.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3tcurkgbt.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3fallwprg.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3clvphfpi.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3qrveebcm.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3ypbzcknn.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3bnehjove.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3kjsbfwqw.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kvabdtvf.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3nlglkzqg.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3hwrjnzhp.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3dkiyxgvj.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3qcvnntol.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3qglfmtfa.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3lctqqxpx.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3omzgnpim.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3jwbmplkf.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3ecjmygft.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3eakyqaud.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3emxcedby.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ltydbrls.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3zhjwixzc.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3vfaudulz.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3yeutczcj.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3rnrksmuc.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3flfzeppx.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3frsopujx.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3junjhevg.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3jgsaoacn.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3bzhpljgt.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3zbwgptsj.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3xznglxty.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3xkjljbpy.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3rumwxxyr.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3tliwlznw.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3gxiwgkwh.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3jvgqybag.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3whvlvavr.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lrwadpfx.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3ukjwgkmi.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3timdjgkv.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3oflyfggp.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3zkefnlal.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3qjrmnjrr.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3tzcynupq.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3voaekywf.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3pctmqltp.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3zwgskmwu.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3ztnohcvh.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3bdcnluut.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3ahulqpng.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3rqwwikdw.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3muvknixm.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3hkvspecv.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3scshgpvm.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3mxywlxqr.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ketrxbrn.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mtnwtegf.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3ifuflgqv.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3acirrsdj.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3llcspoul.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3dobqbmin.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3mrwrestz.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3mgbjlrlm.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3nvyfhonl.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3lcqjekws.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3vbuzxpqd.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3wevdhylc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nzgxettz.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3itjfilyj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3newzyftw.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wlyyhhrq.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3tealopfx.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3twpyzyix.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3zpnwtjmn.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3rvnmqine.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3fiysdxur.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3ovlwqbvb.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3efyqaqtn.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3ldooirxe.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3piltmjao.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3elaearew.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3zzlmbquj.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3mnszkoxm.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3xxuaqker.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3pqihhtub.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3nfkfimec.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3hxjjfhlw.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3ytrddlag.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3pzlnzslj.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3mnubkzjw.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3osgevnla.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3krhbryun.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3oqthaqoo.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3sjesregg.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3ejjezlpt.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3guylabbz.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3usqkrign.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3wofvlbkz.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3zzyrmjlg.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3rmmpvkao.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3iespxkdf.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3rzcmpswl.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3bsdatyno.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3hfyvlfbp.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3xvkgfvsd.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3nioiitwz.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3kueldhms.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3qkqnnqdr.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3ekegooch.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3xtagpdad.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bziruvvz.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3ivjgnioc.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3yoresuce.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3cyesecjd.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3mytjihqh.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3mfhqqegi.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3vjqpllfb.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3zgqgeetw.html


<!-- 参考信息 -->