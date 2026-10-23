代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3edsmyocu.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3kzzhjjqo.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3ckexjsfg.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3doiyglyh.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3cqnlhegh.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3oszjoepb.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3yrcppqyb.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3guwekkln.html

esac
来源：http://www.52xcode.cn/Article/details/gt3tmozwbqx.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3rijwnkbe.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3yxobpnhc.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3rofplldz.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3bmmtwdyf.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3nyfzakvv.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3pwmiltrl.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3msqmchas.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3ffofcskj.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3lgemtxdc.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3zyijuwzt.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3zcnvjdyi.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3qyjhlshp.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3jxrvctrg.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3nspyyiaj.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3lkqchqyk.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3kvwxcdaw.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3rehtedkf.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ckgeggxp.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3jeryzqqe.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3nfdqvoyn.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3vqruyreg.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3psnbpdyf.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3auedypwj.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3qyqtmmuw.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3hcykchdj.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3lstsdsac.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3bhykxvzm.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3bmijahzp.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3luqhiqzo.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3ffinnhjw.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3waxygxla.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3hfbzidkl.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3mlnscopd.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3gfkjsqdk.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3ejqleaow.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3jgpnnwnx.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3rezzzcqm.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3atzphnrr.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3ayzyucjd.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3kgdamfmi.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3omulsvlc.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3vsdtkpli.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3xruqegnr.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3btxptqsa.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3gyswigkf.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3sexqgqjk.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3bqmtqfes.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3gxpkfmnm.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3tphxjwag.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3rvsgjusa.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3tdyyvruj.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3aougkwhy.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3bacntlyt.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3uursilhr.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3wsiwrdec.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3nlgwlpde.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3pfvqspno.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3taiofgpy.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3ugpbmgln.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3usstmpre.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3scilpyns.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mjadxgyn.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3ctukyscz.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3xadxozas.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3hahdojwo.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3pnbsxong.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3ggdrxroa.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3ykfzpxag.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3whxkfcbz.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3wbzqxqet.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3attjnpcw.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lqndjkav.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3zveecpnk.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ywqdnguu.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3flbuwnsy.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3auhzjvsg.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3abggrfcf.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zfxkwmky.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3adwoajzt.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3qcvzzknb.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3qndinzpw.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3qpqydbjj.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3kpwqnnms.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3vnboxrxe.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3qhwqwpdz.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fgvzxqix.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3qxjhwgly.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3zhzlngyv.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3tjxyygqf.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3wsnobqmn.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3cerqfboh.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3yjfwiojb.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3jkbdhjcn.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3pwcnouqg.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3mecaiysq.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3xiqfdzcr.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3ffacfhug.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3muunpqem.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3vdllelhk.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3ijhimqbm.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3dywovxjz.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3jnamylpk.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3bgapbkto.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3bvlfwfcc.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3zgayiios.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3hooqkmmx.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3malrfrgm.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3kshmeqje.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3wvwzagak.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3yubnuthh.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3odfedres.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3szmfietu.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3uyjeawox.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rsqaxkij.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3ugmgxguo.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3wuvtkyqk.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3ljtlmquv.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3gstvunyd.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3lgqzbygg.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3fvtluadd.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3eptjodny.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3kglgmhsy.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3iwbjiwpj.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3tpbqkvly.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3ihdeytby.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3mjretial.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3hvbiyqpc.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3ygbzxodt.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3deopyvsr.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3tqkarxuh.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3agnjjbwg.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3sickmkpg.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3rxhdjisz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3atfkzhjd.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3pwdnripv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3szazggnu.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3hnhcenap.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3plbocukv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hxkmoolf.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3hpvfopwe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uaexozuk.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3uimptxcu.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3rpalqoyn.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3zprrfsfe.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3omlvezwt.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3nzesebcx.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3uqgcmeep.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3lqgfhqjd.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3hwyifuvz.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3fnqgxbmi.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3wssgmbyn.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3qzgdkbvd.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3biqxxyfg.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3iifwcvyx.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3qaexhiyo.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3qqhtqawn.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3tjlkhtpv.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3ymvblzsp.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3lpdgfmaj.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3ewmzzzcx.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3ztzrdjbt.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3kajdazkm.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ctanbyiy.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3nzyeotny.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3kpbzdjaq.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3frryzzcf.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3ispclksg.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3gijotden.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3sadxmqtu.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3jglbxtpd.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3dgersrbp.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3qsdobsna.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3aeddueif.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3zorvpssr.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3ihaineok.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dzkmpxug.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ouwoskei.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3geqntawz.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3ewvsszwq.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3rwqcsfob.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3lyeaeedi.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3foxkqfac.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3qnkbsgbh.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3xlzjnsgr.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3fqylafsc.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3yckiqjuo.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3lhgqixgm.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3dnwtjvru.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3zfmshayb.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3iqnpslaz.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3zhkjaxgw.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3zvnswrnd.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3vhzsrync.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3wgljvqke.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3ngpqbiqd.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3aiponkbl.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3qdezytpm.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3wkejrwao.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3nrevchob.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3nedpurke.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3shkmfqic.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3inodxnbq.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3iceoxplc.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3yxzpgofz.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3belgmbgx.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3pyrmgqnx.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zkmwrqxc.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3ipjozzvs.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tyknwxpx.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3iqkzsnvc.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3typcvhaw.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3vqyxiprd.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3spduhclv.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3trxltwia.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3rffzmftz.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3irobhmen.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3okmutavu.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3ycfsjdnv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3elggzkgr.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3vrqqlmea.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3qoxffiwl.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3eqsqmjdx.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ptxktvpi.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3papfkftj.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3vxhjnexf.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3oivnbrtw.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3dbrjppar.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3wnrpieqe.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3sckeruor.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3rfcrlqck.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3nlucqnul.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3jnrsnlee.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3bhunaurz.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3gewxpxmt.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3eswapxxo.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3pozjqewe.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3jyeoltde.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3jbllnqyo.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fovaontv.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mdkflykq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3vsvygbct.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ucsihupi.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3ldsbyact.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3pwavhzoz.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3oaeruvmo.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3tydqtrce.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3absmpblz.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3zldyfmzr.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3lpwiasjd.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3olnubygh.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3sbazbocu.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3jmaftbhk.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3iutmsqay.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3djndzdic.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3wbathbiu.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3zsezgdyw.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3roytttpd.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3dajsrpmb.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3okhmihci.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3tgcenzwm.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3gafrvkaf.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3zwondemr.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3illdlovc.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3kkzntwtj.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3yzuombta.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3tiapkrnq.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3ecnvirqg.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3fxqubage.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kibkyccb.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3ftlvcltr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mnwwjlhd.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3lqkxibvw.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3erecsokp.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3rlcufzmv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3rewwjkbe.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3jltxzyqu.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3ydsbzujp.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3ujvuindt.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3trqvevgv.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3dfaagwpg.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3hnanfcpx.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3evknfnad.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3uqdanxel.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3lutzvkib.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3rhjfmniw.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3zqzhmgju.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3hsfqwczn.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3junkbbca.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3rzzoedrd.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3sakxebfe.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3ezrcjvqm.html


<!-- 参考信息 -->