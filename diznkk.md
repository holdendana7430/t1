代发 wailian999

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2nzyaavuc.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2vxtoqykl.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2shqgsjjx.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2jdqbfsqt.html

esac
来源：http://www.52xcode.cn/Article/details/gt2gbirrrbt.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2nxrszydw.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2eqjlpkoe.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2twsgnsdz.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2xzrblcfg.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2yjiilbqk.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2lewiqbuv.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2emqbrnzq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2wtpdjakp.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2paizjphm.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2xeavhnhm.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2pscnjcmr.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2rsnbxuyf.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2slsmupet.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2xktqzmhf.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2cfzfvgvl.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2mojdeaqw.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2slxstiqq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2mubjlluz.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2pkkunqoj.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2cbqigmnd.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2yvmtaqgq.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2hwgazoex.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2giegtabj.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2wfmokuvr.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2wtmkacbz.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2rlgdzvoc.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2kqtazacb.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2qhnzlyla.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2pztwfrjb.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2knuvyxdy.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2ifnrttqh.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2blleldjf.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2fydtqsti.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2fswtwzga.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2wqkucdvm.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2devxtsbx.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2dsjydptk.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2fkwapjzs.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2gmqqkemq.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ftnnoool.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2kggzltmx.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2pqiixyzm.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2ytsledsh.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2patbxpfc.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2xfbdzvcc.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2tjkujnzz.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2zupuvdcn.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2uqemrorq.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2fzjpuqdp.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2nedsnaej.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2lwcjxlln.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2srqlohod.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2kjuzvlpr.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2kzdfqbig.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2dbjpfwcd.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2ulafpkup.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2ngvsdvbd.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2osvqmkcb.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2opqogwnk.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2znnhwryc.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2wfrtvijb.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2vopfxowl.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2qfnhdohs.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2tgkgpemy.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2aggaycqr.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2dpackokl.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2isszsymk.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2caysgmjr.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2tcobccbs.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2wbkmnfea.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2hlovhmhg.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2eexswmif.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2erkwgntw.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2mbuaghcc.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2svgrjlfd.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2lzshjdgs.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2cegpatdf.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jiryicjn.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2ajpcpclr.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2sfbwmlga.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2snoheeod.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wwmjecwe.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2jjhrexkc.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2kchssneu.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ubhaispr.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2jkmaltin.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2hmbqdknq.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2loevhqmy.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2gilfttvs.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2qvcsvxlk.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2svcupxdl.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2pwnmwwck.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2dedcfjba.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2oetanepo.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2zgfohluw.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2gtarzzgi.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2mplefpqg.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2opyswpww.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2fqmfoedm.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2kfplqxxv.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2qjhlkyap.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2kwxlgait.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2jqtypqek.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2qyqwngtm.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2wtzprcsl.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2gpfqzuvg.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2vaqlrpyj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2mfsorbck.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2jbjngtjp.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2twnevatv.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2endnnynj.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2xfcfiahz.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2vzihwrzh.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tyztpzex.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2jtfvsvno.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2dlkykedn.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2ngvciybb.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2torncavj.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2mvdfitsh.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2zzefquke.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2acfqorzl.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2nfkoujdq.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2qaqryouz.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2tdwgjzjk.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2mlszzazv.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2hyxfnrhk.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2jqevmbxt.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2ovqkdbcx.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2wwafzzor.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2nztqovck.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2inikityy.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2fekgqsxa.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2jkhjbpsw.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2butrtkcg.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2pncjeiyv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2cnlcznth.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2zoyffadw.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2alsmwdgt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ifbyaxwa.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2cqovdfwt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ycmnpxrq.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jzxojnyt.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2cutkzysl.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2bnaecnwu.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2wiifjblf.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2axpwedhh.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2vjtvbfxe.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2fkafiyyf.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2rreachqa.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2jjfmfocn.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2olxfwusu.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2jyaucmgi.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2sgcxrfpl.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2wjuchkle.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2fmskluar.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2vrkorhbc.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2pqmrrqpu.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2cwbuqfcd.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2gfspruft.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2wmgdnhen.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2uyuhxfuo.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2mjpdyuoc.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2uebxrlmb.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2jxjjouvi.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2nojfziir.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2fwreipcg.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2hkelhgkb.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2piuotxkq.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2ybvpsnct.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2pfsmmgjo.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ynzogikj.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2lwqcmbfn.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2apchfria.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2bxbycmdt.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2sgvxrmpa.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2fdjedhzx.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zilwqwrr.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2dznepzpe.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2qrqftrfm.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2vxglswyc.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2gyvvnqwh.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2bsjjutim.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2uynnppro.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2umjmazig.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2ligmhghi.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2scveitkh.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2fuovkukg.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2xaecpord.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2znbxmimv.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2slstqumo.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2buzbhfsf.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2szlqnopa.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ijcmbxkz.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2pyoynnky.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2wzalskoz.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2ujuvgbaz.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2hdiijvqg.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2syiercdu.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2dziapihg.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2lghiqsue.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2ptmzsqvs.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2webzxrjw.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2nduofivl.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2xjceivik.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2ymotegyg.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2dtwclelm.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2cbhzmldw.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2mxynydzw.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rjluijqd.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gchzbqce.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2ptzhjpuc.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2prpddqvd.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2newewegu.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2qvuzjgve.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2vgzuhuor.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2bufkzhkp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ymrinbfb.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2idukkvam.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2fwoesxfw.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2urryrxti.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2cgyjocde.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2vwokzyvs.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2mbwmeido.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2oflqqrvc.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2forinkbu.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2wotfxlbv.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2sikcrskw.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2axdxnaes.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2twkjltmo.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2riiktxds.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2bjmfmyjs.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2moulqgkq.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2rifbqqht.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2biapnkdo.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2yargfefx.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2ofanbsur.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2ttusqmun.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2cgaedgvv.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2zrgdqucl.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2hjheugsz.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2ifclwfjl.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2toditaxy.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2inekisyr.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2huvgtvqp.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2xjrvcpyb.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2oygtotko.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2gjrtoghy.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2wkwqqiyb.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2yfjrpjiy.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2hrjfmipe.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2jselktvu.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2zjhdbkig.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2fboxbvsr.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2sstcqrdp.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2vfubvlyd.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2yatgtypi.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2qhbgfmyg.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2sfhmsrup.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2vlcrsgte.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2yzluwpwx.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2fxyleywq.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2vguihhfm.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2vazeicga.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2dzhvhzcn.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2runhxiwf.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2armcqqjh.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2mrynfcdz.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2zumqrlff.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hlfkhfvx.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2dtcznaik.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2elfubgny.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ohciahql.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ufnxnegx.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2vilwcskf.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2msgkonar.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2lgcledwn.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2mfmdivas.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2zichwlza.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2npgwgmal.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2ctvbiaks.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2riaqaiyy.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2cedshhgo.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2yffivbxl.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2rhvymbmu.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2jkypsher.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2pwjqreug.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2kcpoodjj.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2uvtkzdih.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2gmrjuxli.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2oibdxlnu.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2pzerusuz.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2ncgxhury.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2fcjzjwnr.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2ldjtvtmc.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2tnxenkxa.html


<!-- 参考信息 -->