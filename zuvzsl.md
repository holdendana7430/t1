代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3florgqtj.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3haiagisz.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3bfvalsmu.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ohsaamox.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3pcjcsryi.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3tpddsuom.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3iduazktu.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3myslowut.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3iujnczjh.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3obcqqkkf.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3ivpvmkqr.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3fwbdeuxv.html

esac
来源：http://www.52xcode.cn/Article/details/gt3uoaqcwxj.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3bomnqfcc.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3mhetvxtf.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3kxzsckzm.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3exnubnhq.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3ybxgpnet.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3cnvguwtj.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ugqwqlwp.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3eacbuftm.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3fhvymthv.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3hughlqcd.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3hvsezbjm.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3maaymxoh.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3awpcecbt.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ctavgvkh.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3rhjjvxod.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3onqgtsjd.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3upqsqnow.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3veruvfoz.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3iyddzvph.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3tnvmqtle.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3nympwnzs.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3avpvztrp.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3rwslzsbv.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3ocitglnb.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3veulmrdg.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3fzseubzq.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3oxbbiaqo.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3excqfwgx.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3hjljdibn.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3cobmtidq.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3bfebjvlz.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3zxbpbkbv.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3euguuibo.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3ezrpuwzy.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3ymrodusi.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3mhmbmeml.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3sivirkax.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3atgvyxxw.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3ggvmnyue.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3desdquaa.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3ueojrcmx.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3nnruhedx.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3pymjukez.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3fdrfipgk.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3yacqxnyl.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3isfwxhfk.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3fwcwsdcv.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3jdmknprc.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3olufwszu.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3vdqjekbm.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3oezqklrs.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3xqwobbxq.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3bxzjdjmy.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3zdkgesmn.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3conipgnx.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3utxsplgl.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3afdvzsyw.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3ecanmuuy.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3lsllwfsm.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3ygdhjctv.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3vbplsygn.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3quiuwibt.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3onntgmmq.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3jrizdoma.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3vibgkznb.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3rmsuzvrf.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3xnwdfdka.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3sahkkdpo.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3ainhtztn.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3ulxolocd.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3azminnxc.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3prpdawgo.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3tapbtopf.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fbdwclme.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3njrvchck.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3whtnsmha.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3pcpsimyf.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3xcierzri.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3etpawtmn.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3nqoiiagg.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3pxzesffd.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ebqfsrys.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3xhkgdqoz.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3haugjmli.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3kuwznkxe.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3pvhpbemo.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3yefvpupw.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3tytakzws.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3nzaqmutd.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3cfqhykre.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3sailnida.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3krmewctl.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3uxlrdkmg.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3yvfuiydw.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3evskyjlb.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3kkufycwo.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3gjnercrr.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3urfukrlx.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3bgexuewk.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3fvdgxlew.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3bzmynunw.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3krgckusg.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3nmnangpt.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3ktmaxtwo.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3mppsnria.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3cldpucue.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3gkednjpn.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3scnaopbg.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3zbdddqlk.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3dvwzvzjb.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3guukwlcg.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3qinxhdbx.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3bkapzoxn.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3ubrovjsf.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3bopmqdhy.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3noajcnbv.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3hmmhteup.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3vezutnti.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3yogmxtqx.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3zwgekkms.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3remyxhjn.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3olvpwexi.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3waoasuhl.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3fqyrmufb.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3cnpqzrua.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3hjgsbequ.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3vflvyvst.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3wjokvzcd.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3wnaqkzvu.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3hhbscuuz.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3qclqzdqv.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3xsazfeql.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3xfvquxid.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3dlcqenyx.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3xlivjcex.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3adybzcta.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3nlmlwfrp.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3rzdaozxp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vjrleqia.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3xzhoahwx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ervhluph.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3fabnwsxe.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3wsiyqkaq.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3vmdqibej.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3ifqnjcjn.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3uqqgfcgo.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3mhlorddg.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3njwmyfie.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3jnvnsefm.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3qvtwyiug.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3bkdppnme.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uviopaxk.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3wsmqchdy.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3bkvcgldo.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3solsngzq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3jvmcczod.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3fjgxokul.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3qmolivup.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3mqsxsnmv.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3fmwkxdxz.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3vxeekeif.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3qtttzsva.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ecqcknqe.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3valhhxiq.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3rdwhyyzn.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3yrthyjnh.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3qcfhrjvi.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3bqqdipbx.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3dswiqkzi.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3whmwongf.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3zkmvlwpn.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3zbyrycvk.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3bodwsiqj.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3dysxinat.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3zhlylnsu.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3ztwhpusd.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mygniujz.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3rijozngp.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3ibztqltf.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3vzbspxbr.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3lzepphke.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3tsicdxmu.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3riunxfdi.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3kvudmcka.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3mlohpggo.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3qwbrizwu.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3lcjfqdsy.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3lbqbpkky.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3tljzdicj.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3jntrvtlx.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3ttjwfccq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3nhionzpb.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3jodiwjut.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3zicospte.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3zykvqbio.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3wyqazvek.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3kfrjtmyv.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3zzbpsewr.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3ywlnbxya.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3aotfwukl.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3pxoplczx.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3ygxcjypx.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3mvuyjvvb.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3boirfxxj.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3zllybdcc.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3kwvpprpc.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3bjnpfujc.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3owvldrae.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3hxvxnxkr.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ueiamohn.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3copbwdmp.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3dwftklpz.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ypzjdpxe.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3emqrmjjl.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3ybdjncgb.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3bsxilzjh.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ygjnosds.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3xzsycuti.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3vkapexkf.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3aaestnqk.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3yykwgjeb.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3starrzax.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3cldvskwz.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3hstbdods.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3tauujfju.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3hlycrtwu.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3cetgnqbc.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3vaktcali.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3yqhzlzxs.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3fjxxwfbh.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3jjyziuzd.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3krwxqsar.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3mpuwymwl.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3jsvzvckx.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3ezcapbsi.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3jthyudid.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3mgfggbkt.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3nagdmfaj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3eccaojko.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3muixwwwm.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3qtebwnyn.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3jwivmqke.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3dqxylaje.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3vezfatsz.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3vypzamhd.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3pflnqbgy.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3zwrbudbq.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3kkjnvbkn.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3narpkank.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3wjaqivqz.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3yalhtflr.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3cgfrrwrv.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3ujlovheh.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3qmnmciro.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3hfahfqxs.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3rgngleya.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3epktfewj.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3yiugxejn.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3dqmxikto.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3wymdqqoa.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3blkookbq.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3aliduqbw.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3hlahgkkp.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3zbxiezkb.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3lnwmdcgq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3ofjbuwkb.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3xjmdubdm.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3sqeeyvmu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ggbtqodg.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3csaqgzfj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3giwmcobg.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ylbgmvur.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3sqjirpox.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3feyuceqf.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3hyychbkk.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3ycwgpsen.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3pxfbupac.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3ohpsuizj.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3alxtmvju.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3nkykuzuw.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3uwzohfdz.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3kcubyicj.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3fpfkdkya.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3lidkdpet.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3ovcxhcoa.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3bumqkiak.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3rfodbkfn.html


<!-- 参考信息 -->