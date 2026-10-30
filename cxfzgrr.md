代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fehbvm.com/Article/details/gyashzgxb.sHtML

[R10] 正则匹配
来源：http://baike.hesvh.cn/Article/details/gcjwgwfcg.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.hesvh.cn/Article/details/gbjjrryhv.sHtML

[R11] case 多分支
来源：http://www.m.share.zdbjq.cn/Article/details/gooyyxvvc.sHtML

case "$1" in
来源：http://m.share.hesvh.cn/Article/details/giuupzsfg.sHtML

start) echo "启动" ;;
来源：http://m.share.zdbjq.cn/Article/details/gmrjwdmfy.sHtML

stop)  echo "停止" ;;
来源：http://mobile.zdbjq.cn/Article/details/gaadyvrvf.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fehbvm.com/Article/details/gxsxxdrrn.sHtML

esac
来源：http://www.m.share.hesvh.cn/Article/details/guxtkpzfm.sHtML

[R12] for 遍历文件
来源：http://read.share.hesvh.cn/Article/details/gfvqhkhbz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.hesvh.cn/Article/details/gdsrsopga.sHtML

[R13] for 计数循环
来源：http://www.share.fehbvm.com/Article/details/gbmmvcovx.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/ggkvlkkqh.sHtML

[R14] C 风格 for
来源：http://read.share.zdbjq.cn/Article/details/gprhtromg.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/ggztvfmtj.sHtML

[R15] while 逐行读文件
来源：http://wap.fehbvm.com/Article/details/ghahufwve.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.hesvh.cn/Article/details/ghfnyvhsn.sHtML

[R16] until 等待条件
来源：http://blog.zdbjq.cn/Article/details/grgwnzuku.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/gfsoarksy.sHtML

[R17] 数组定义与取值
来源：http://www.share.hesvh.cn/Article/details/gigkdyyqn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.hesvh.cn/Article/details/gsnysizmf.sHtML

[R18] 遍历数组
来源：http://baike.fehbvm.com/Article/details/gaugsadcy.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fehbvm.com/Article/details/gfdqslemy.sHtML

[R19] 数组长度
来源：http://baike.hesvh.cn/Article/details/gbyepgvgi.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fehbvm.com/Article/details/gpjxdxfpi.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.zdbjq.cn/Article/details/ghucjwvxn.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.zdbjq.cn/Article/details/gjfqdodhw.sHtML

[R21] 字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/gcetnkohs.sHtML

echo "${#s}"
来源：http://3g.zdbjq.cn/Article/details/gjvtluuss.sHtML

[R22] 截取子串
来源：http://wap.zdbjq.cn/Article/details/ghynzuwnv.sHtML

echo "${s:0:5}"
来源：http://wap.fehbvm.com/Article/details/gbgvfwotn.sHtML

[R23] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/gqahfjlua.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.hesvh.cn/Article/details/gpkngwsdq.sHtML

[R24] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/gbohosldz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.hesvh.cn/Article/details/gkgwinkuz.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.hesvh.cn/Article/details/grrlxqyje.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.zdbjq.cn/Article/details/geodzmjna.sHtML

[R26] 命令替换
来源：http://read.share.hesvh.cn/Article/details/gfpitccvk.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.hesvh.cn/Article/details/gkxejhteh.sHtML

[R27] 算术展开
来源：http://read.share.fehbvm.com/Article/details/grgkvycpf.sHtML

echo $((1 + 2 * 3))
来源：http://blog.zdbjq.cn/Article/details/gwawfteto.sHtML

[R28] 浮点运算
来源：http://www.blog.zdbjq.cn/Article/details/gqeaoozku.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.hesvh.cn/Article/details/gkohzcgpe.sHtML

[R29] 定义函数
来源：http://mobile.fehbvm.com/Article/details/ggdydagpx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.hesvh.cn/Article/details/gidmoiryf.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.hesvh.cn/Article/details/gbtoqiqsb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.hesvh.cn/Article/details/gozyzhsfc.sHtML

[R31] 局部变量
来源：http://m.share.fehbvm.com/Article/details/gybejxhih.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.hesvh.cn/Article/details/gpzbywyjs.sHtML

[R32] 参数个数校验
来源：http://www.share.hesvh.cn/Article/details/gmlinmzkd.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.hesvh.cn/Article/details/gkpnpqycy.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.hesvh.cn/Article/details/gyiovtnui.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.zdbjq.cn/Article/details/gcikcbfkg.sHtML

[R34] 退出时清理
来源：http://www.share.hesvh.cn/Article/details/gzcmokksj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fehbvm.com/Article/details/gickyydlo.sHtML

[R35] 后台执行并等待
来源：http://blog.fehbvm.com/Article/details/ggbwarfve.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.hesvh.cn/Article/details/grxkmidli.sHtML

[R36] 并发执行多个任务
来源：http://baike.zdbjq.cn/Article/details/gcnncxuij.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.zdbjq.cn/Article/details/gujucflxu.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.zdbjq.cn/Article/details/gvdbefuue.sHtML

files=$(ls -1)
来源：http://mobile.zdbjq.cn/Article/details/guwqzpdwu.sHtML

[R38] 管道串联
来源：http://read.share.zdbjq.cn/Article/details/gsiwddalk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.zdbjq.cn/Article/details/gdurlipeq.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fehbvm.com/Article/details/ggmbbwpwl.sHtML

cmd > out.log 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/grruaznke.sHtML

[R40] 追加写日志
来源：http://www.share.zdbjq.cn/Article/details/gqhdiujve.sHtML

echo "log" >> out.log
来源：http://blog.fehbvm.com/Article/details/gsnrkxjep.sHtML

[R41] 丢弃输出
来源：http://baike.hesvh.cn/Article/details/gccdhrmjw.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.hesvh.cn/Article/details/gmupkeaay.sHtML

[R42] 输入重定向
来源：http://www.m.share.zdbjq.cn/Article/details/ggolshjio.sHtML

wc -l < a.txt
来源：http://baike.hesvh.cn/Article/details/gkfneqwse.sHtML

[R43] 按名字查找文件
来源：http://mobile.hesvh.cn/Article/details/gpfindqtv.sHtML

find . -name "*.log" -type f
来源：http://wap.hesvh.cn/Article/details/gmuiwkmoq.sHtML

[R44] 按修改时间查找
来源：http://www.blog.zdbjq.cn/Article/details/gpqwumaaa.sHtML

find . -mtime -7 -type f
来源：http://www.share.fehbvm.com/Article/details/gzgzpbdcl.sHtML

[R45] 批量删除
来源：http://read.share.hesvh.cn/Article/details/gcvbsswfr.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.zdbjq.cn/Article/details/gcfaqfapq.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fehbvm.com/Article/details/gcktritbk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.hesvh.cn/Article/details/gowzmgxzr.sHtML

[R47] sed 单行替换
来源：http://read.share.zdbjq.cn/Article/details/gevnqvvkm.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.hesvh.cn/Article/details/gsgszkskw.sHtML

[R48] awk 取指定列
来源：http://www.m.share.hesvh.cn/Article/details/gyduidsrp.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fehbvm.com/Article/details/gcpgelyfm.sHtML

[R49] awk 带条件
来源：http://3g.zdbjq.cn/Article/details/gocqevajf.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fehbvm.com/Article/details/gyluapqzg.sHtML

[R50] awk 求和
来源：http://www.m.share.hesvh.cn/Article/details/gsntrsxon.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.zdbjq.cn/Article/details/guhaokgge.sHtML

[R51] 排序去重取前几
来源：http://m.share.zdbjq.cn/Article/details/geddlszpv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.zdbjq.cn/Article/details/gdaagnols.sHtML

[R52] 统计行数
来源：http://mobile.fehbvm.com/Article/details/gsqnfphun.sHtML

wc -l a.txt
来源：http://read.share.zdbjq.cn/Article/details/gubdbxozn.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.zdbjq.cn/Article/details/gxtsebmxj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.zdbjq.cn/Article/details/geplzaaon.sHtML

[R54] 比较两个文件
来源：http://baike.zdbjq.cn/Article/details/gyonmhofs.sHtML

diff a.txt b.txt
来源：http://www.blog.fehbvm.com/Article/details/glodsbszm.sHtML

[R55] 压缩与解压
来源：http://www.blog.zdbjq.cn/Article/details/gsavsrwlk.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fehbvm.com/Article/details/gechixrcy.sHtML

[R56] 远程拷贝
来源：http://blog.hesvh.cn/Article/details/glqugpucs.sHtML

scp file user@host:/path/
来源：http://wap.hesvh.cn/Article/details/gogaslonk.sHtML

[R57] 远程执行命令
来源：http://m.share.fehbvm.com/Article/details/gpiakqfjj.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fehbvm.com/Article/details/gkguujsez.sHtML

[R58] 下载文件
来源：http://wap.zdbjq.cn/Article/details/gswpmvzfz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.hesvh.cn/Article/details/gukrkrrlf.sHtML

[R59] 发 POST JSON
来源：http://blog.fehbvm.com/Article/details/gjylmdwjz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.hesvh.cn/Article/details/gbwlmwsyg.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/gafxywsbb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fehbvm.com/Article/details/godfdenks.sHtML

[R61] 磁盘占用
来源：http://www.blog.fehbvm.com/Article/details/gtmhssyau.sHtML

df -h;  du -sh *
来源：http://www.share.fehbvm.com/Article/details/gnovdwpih.sHtML

[R62] 找最占空间的文件
来源：http://3g.zdbjq.cn/Article/details/gaunoabyw.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.hesvh.cn/Article/details/gcjbbnixm.sHtML

[R63] 内存与进程
来源：http://blog.zdbjq.cn/Article/details/gvgbdnfst.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.hesvh.cn/Article/details/galizbwxg.sHtML

[R64] 结束进程
来源：http://wap.zdbjq.cn/Article/details/gelvezgom.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fehbvm.com/Article/details/gzjrsmdae.sHtML

[R65] 查看端口占用
来源：http://wap.fehbvm.com/Article/details/gnotpsfmn.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.hesvh.cn/Article/details/gwdzxcexu.sHtML

[R66] 定时任务
来源：http://www.m.share.hesvh.cn/Article/details/gnytxqxtr.sHtML

crontab -e;  crontab -l
来源：http://www.blog.hesvh.cn/Article/details/gawgtfytd.sHtML

[R67] 生成随机十六进制串
来源：http://blog.zdbjq.cn/Article/details/gpvnsnllu.sHtML

openssl rand -hex 16
来源：http://m.share.fehbvm.com/Article/details/gtlaqvbdb.sHtML

[R68] 计算文件校验值
来源：http://www.share.hesvh.cn/Article/details/gcbapkiki.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fehbvm.com/Article/details/gyxwgylhf.sHtML

[R69] 生成随机密码
来源：http://www.share.fehbvm.com/Article/details/gntnqiycm.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.hesvh.cn/Article/details/gwxxozwkp.sHtML

[R70] 时间戳与互转
来源：http://www.share.zdbjq.cn/Article/details/gbosaznms.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.hesvh.cn/Article/details/gufhitsym.sHtML

[R71] 日期格式化
来源：http://baike.hesvh.cn/Article/details/gmowhebyx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.hesvh.cn/Article/details/ggknuttsw.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fehbvm.com/Article/details/gcjxxxiyj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/ggftldhmm.sHtML

[R73] 分割大日志
来源：http://www.share.zdbjq.cn/Article/details/gqkdggkke.sHtML

split -l 1000 big.log part_
来源：http://3g.fehbvm.com/Article/details/gggofcvgw.sHtML

[R74] 批量重命名
来源：http://mobile.hesvh.cn/Article/details/gaoiidisj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.hesvh.cn/Article/details/gfrnvkwtj.sHtML

[R75] 导出环境变量
来源：http://read.share.fehbvm.com/Article/details/gfbhfohhi.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.hesvh.cn/Article/details/gakyccnti.sHtML

[R76] 使用临时文件
来源：http://www.m.share.hesvh.cn/Article/details/gcnqyweix.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/gjpfgljjc.sHtML

[R77] 读取用户输入
来源：http://3g.fehbvm.com/Article/details/gntvcvupv.sHtML

read -rp "请输入: " ans
来源：http://mobile.zdbjq.cn/Article/details/glzcfwmwl.sHtML

[R78] 交互式菜单
来源：http://baike.fehbvm.com/Article/details/grmgaujlx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.hesvh.cn/Article/details/glocrhabg.sHtML

[R79] 解析命令行选项
来源：http://www.blog.zdbjq.cn/Article/details/geocxbvyz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.hesvh.cn/Article/details/gwqjwryca.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.zdbjq.cn/Article/details/gpsgcynjb.sHtML

time ./run.sh
来源：http://3g.fehbvm.com/Article/details/gcwaqlnge.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gmdekfjdh.sHtML

S. C / C++ 专题
来源：http://www.blog.zdbjq.cn/Article/details/guxghotfe.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gbeonuoup.sHtML

[S01] C：Hello World
来源：http://www.share.hesvh.cn/Article/details/glrhapryh.sHtML

#include <stdio.h>
来源：http://www.m.share.zdbjq.cn/Article/details/gzoectgjp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.zdbjq.cn/Article/details/gazvbkuvr.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.zdbjq.cn/Article/details/gfywszeag.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.hesvh.cn/Article/details/gyvzvxulh.sHtML

[S03] C：读入整数
来源：http://www.m.share.zdbjq.cn/Article/details/gpeotccoi.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.zdbjq.cn/Article/details/gxskxxoro.sHtML

[S04] C：字符串复制
来源：http://blog.zdbjq.cn/Article/details/gapnttpib.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fehbvm.com/Article/details/gaelgnerr.sHtML

[S05] C：字符串长度
来源：http://www.share.fehbvm.com/Article/details/gdzqgjuew.sHtML

strlen(s)
来源：http://baike.fehbvm.com/Article/details/gkemnchbe.sHtML

[S06] C：字符串比较
来源：http://m.share.fehbvm.com/Article/details/gdolciavg.sHtML

strcmp(a, b) == 0
来源：http://read.share.zdbjq.cn/Article/details/gsfhgbpyb.sHtML

[S07] C：数组遍历求和
来源：http://m.share.zdbjq.cn/Article/details/guonxshvz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fehbvm.com/Article/details/gypkpztdl.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fehbvm.com/Article/details/grzqmyxiu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.hesvh.cn/Article/details/gxocsegth.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.zdbjq.cn/Article/details/goaxmlvol.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.zdbjq.cn/Article/details/gfmqpkhdc.sHtML

[S10] C：指针与解引用
来源：http://www.share.zdbjq.cn/Article/details/gutnauked.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fehbvm.com/Article/details/gcmtacakp.sHtML

[S11] C：逐行读文件
来源：http://3g.hesvh.cn/Article/details/guadctjgt.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.zdbjq.cn/Article/details/guxrcvvad.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fehbvm.com/Article/details/gjmflicth.sHtML

fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/ghrrfbczi.sHtML

[S12] C：写文件
来源：http://mobile.hesvh.cn/Article/details/grolsqsuq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/gvvztttpu.sHtML

[S13] C：宏定义
来源：http://m.share.fehbvm.com/Article/details/gpdbjwomy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.hesvh.cn/Article/details/gdcjqkjwe.sHtML

[S14] C：枚举
来源：http://wap.zdbjq.cn/Article/details/gfnsnykie.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.hesvh.cn/Article/details/giupphcsr.sHtML

[S15] C：类型转换
来源：http://read.share.hesvh.cn/Article/details/gtwcwclme.sHtML

(double) a / b
来源：http://3g.zdbjq.cn/Article/details/gxpipvbjx.sHtML

[S16] C：位操作置位
来源：http://m.share.hesvh.cn/Article/details/gwxalvoah.sHtML

x |= (1 << 3);
来源：http://www.m.share.fehbvm.com/Article/details/gxygbmqtz.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fehbvm.com/Article/details/ginncadfr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.zdbjq.cn/Article/details/gshwmkuab.sHtML

[S18] C：命令行参数
来源：http://www.share.zdbjq.cn/Article/details/gjcfftnjk.sHtML

int main(int argc, char **argv)
来源：http://read.share.zdbjq.cn/Article/details/gzkfanenv.sHtML

[S19] C：快速排序
来源：http://www.share.zdbjq.cn/Article/details/gkniwrddb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/gxsswhxbw.sHtML

[S20] C：二分查找
来源：http://m.share.hesvh.cn/Article/details/gxewbynff.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/gwlkdkcng.sHtML

[S21] C：字符类别判断
来源：http://3g.hesvh.cn/Article/details/gzybapfyj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fehbvm.com/Article/details/gsewhjgva.sHtML

[S22] C：字符串转数字
来源：http://www.share.zdbjq.cn/Article/details/gvbtahibx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.hesvh.cn/Article/details/geiiyezlg.sHtML

[S23] C：随机数
来源：http://baike.zdbjq.cn/Article/details/grcojiilp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.zdbjq.cn/Article/details/ghqjusqlr.sHtML

[S24] C：获取本地时间
来源：http://3g.fehbvm.com/Article/details/gqqwiwxqk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.hesvh.cn/Article/details/gdudjdawv.sHtML

[S25] C：内存拷贝
来源：http://www.share.hesvh.cn/Article/details/gsrmelmep.sHtML

memcpy(dst, src, n);
来源：http://read.share.fehbvm.com/Article/details/gkllaecrk.sHtML

[S26] C：内存清零
来源：http://mobile.fehbvm.com/Article/details/gxxfvzird.sHtML

memset(a, 0, sizeof a);
来源：http://3g.hesvh.cn/Article/details/gwtgzpcwk.sHtML

[S27] C：定义常量
来源：http://blog.hesvh.cn/Article/details/gqvvmamts.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/glsldmcxv.sHtML

[S28] C：静态变量
来源：http://m.share.hesvh.cn/Article/details/graxqxrvj.sHtML

static int counter = 0;
来源：http://read.share.zdbjq.cn/Article/details/gbsqcujuz.sHtML

[S29] C：变参函数
来源：http://wap.fehbvm.com/Article/details/gjgejtrqo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.zdbjq.cn/Article/details/gwobronlk.sHtML

[S30] C：头文件保护
来源：http://www.m.share.hesvh.cn/Article/details/gevbjieqe.sHtML

#ifndef X_H
来源：http://mobile.hesvh.cn/Article/details/gqdaaowkg.sHtML

#define X_H
来源：http://3g.fehbvm.com/Article/details/gsepfvhva.sHtML

#endif
来源：http://mobile.hesvh.cn/Article/details/galslmajb.sHtML

[S31] C++：Hello World
来源：http://m.share.hesvh.cn/Article/details/gphipahqb.sHtML

#include <iostream>
来源：http://www.share.fehbvm.com/Article/details/gpgkxkrgv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.hesvh.cn/Article/details/gutyfiuqk.sHtML

[S32] C++：字符串
来源：http://wap.fehbvm.com/Article/details/gjmvjnidk.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fehbvm.com/Article/details/gyiahezvm.sHtML

[S33] C++：vector 增删
来源：http://wap.hesvh.cn/Article/details/gidyciyxq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fehbvm.com/Article/details/gqnvesvse.sHtML

[S34] C++：遍历 vector
来源：http://www.share.zdbjq.cn/Article/details/gqwedmpfr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.hesvh.cn/Article/details/gruldslws.sHtML

[S35] C++：map
来源：http://3g.zdbjq.cn/Article/details/gtpmssaom.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/glvrboqjr.sHtML

[S36] C++：unordered_map
来源：http://www.blog.zdbjq.cn/Article/details/gntijoiol.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/gqzygkzoi.sHtML

[S37] C++：set
来源：http://baike.zdbjq.cn/Article/details/ggmmbqtnu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.zdbjq.cn/Article/details/gghbmxklh.sHtML

[S38] C++：排序
来源：http://m.share.fehbvm.com/Article/details/gxzyvojlh.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fehbvm.com/Article/details/gcsvsqdjw.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.hesvh.cn/Article/details/grhlsjpqv.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.hesvh.cn/Article/details/gnneqcihi.sHtML

[S40] C++：查找元素
来源：http://read.share.zdbjq.cn/Article/details/grhbqdlgy.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fehbvm.com/Article/details/gaaqcxgld.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gjigralfc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fehbvm.com/Article/details/gvnvazysw.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.zdbjq.cn/Article/details/gkaujfrxh.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fehbvm.com/Article/details/gcbxeonqy.sHtML

[S43] C++：智能指针
来源：http://www.blog.zdbjq.cn/Article/details/gifewhkvm.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.hesvh.cn/Article/details/gxtejnpsq.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fehbvm.com/Article/details/gzmslqozj.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fehbvm.com/Article/details/gcvebtopw.sHtML

[S45] C++：lambda
来源：http://read.share.hesvh.cn/Article/details/ggkvzgnaj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.hesvh.cn/Article/details/gtcmcedot.sHtML

[S46] C++：函数模板
来源：http://mobile.hesvh.cn/Article/details/gddpqfnqn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fehbvm.com/Article/details/gihrjscbz.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.zdbjq.cn/Article/details/gztonyfhz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.zdbjq.cn/Article/details/gtkkbwoco.sHtML

[S48] C++：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gylvoxwpz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.zdbjq.cn/Article/details/ggrfujuzj.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fehbvm.com/Article/details/ggxpkzlkm.sHtML

[S49] C++：写文件
来源：http://3g.fehbvm.com/Article/details/gmqscjght.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.hesvh.cn/Article/details/gidemafly.sHtML

[S50] C++：格式化数字
来源：http://wap.fehbvm.com/Article/details/gcbevtvfs.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fehbvm.com/Article/details/gfjrdmrvw.sHtML

[S51] C++：显式类型转换
来源：http://baike.zdbjq.cn/Article/details/gejhinann.sHtML

static_cast<double>(a) / b
来源：http://www.blog.hesvh.cn/Article/details/gdajdsevn.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.zdbjq.cn/Article/details/girnvqhex.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.hesvh.cn/Article/details/gwjgyugpe.sHtML

[S53] C++：移动语义
来源：http://baike.zdbjq.cn/Article/details/gjgxfvsac.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fehbvm.com/Article/details/gozvdxaig.sHtML

[S54] C++：异常处理
来源：http://www.blog.hesvh.cn/Article/details/gejpeoynw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.zdbjq.cn/Article/details/gtgmxhuxv.sHtML

[S55] C++：结构化绑定
来源：http://blog.fehbvm.com/Article/details/guskksuow.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.hesvh.cn/Article/details/gnjvmzabc.sHtML

[S56] C++：optional
来源：http://blog.zdbjq.cn/Article/details/gxsenhzmp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.zdbjq.cn/Article/details/gljhjdzez.sHtML

[S57] C++：编译期常量
来源：http://m.share.zdbjq.cn/Article/details/govwhyqnd.sHtML

constexpr int N = 10;
来源：http://wap.zdbjq.cn/Article/details/gcymtbdjm.sHtML

[S58] C++：命名空间
来源：http://read.share.zdbjq.cn/Article/details/gkezbznhq.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fehbvm.com/Article/details/gcfjxmcvm.sHtML

[S59] C++：静态断言
来源：http://www.share.hesvh.cn/Article/details/gfkqaverj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fehbvm.com/Article/details/gmkgeytes.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.zdbjq.cn/Article/details/gexewyswh.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fehbvm.com/Article/details/gnepfeuov.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gjigytjcx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fehbvm.com/Article/details/gopfwdtfd.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gtyjmzuuq.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gicbfifpk.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/gknwuasmd.sHtML

[T02] Kotlin：变量
来源：http://www.blog.zdbjq.cn/Article/details/gnvktydok.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.hesvh.cn/Article/details/grswyqeuq.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.hesvh.cn/Article/details/gkgspfyzo.sHtML

"值: $b"
来源：http://www.m.share.zdbjq.cn/Article/details/glrjrkwuv.sHtML

[T04] Kotlin：空安全
来源：http://m.share.hesvh.cn/Article/details/gimqaybnc.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.zdbjq.cn/Article/details/gmzdxozbh.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fehbvm.com/Article/details/gpzbzlbnp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.zdbjq.cn/Article/details/gdujqumzo.sHtML

[T06] Kotlin：集合映射
来源：http://wap.zdbjq.cn/Article/details/gfimeuntc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gmtgonwex.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.hesvh.cn/Article/details/gftgesbcj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.hesvh.cn/Article/details/gyzavsnan.sHtML

[T08] Kotlin：数据类
来源：http://wap.fehbvm.com/Article/details/gdberwtjr.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.zdbjq.cn/Article/details/gfvrguxzg.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.zdbjq.cn/Article/details/gejnjqewb.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.zdbjq.cn/Article/details/gsfqiqdgo.sHtML

[T10] Kotlin：默认参数
来源：http://3g.hesvh.cn/Article/details/gnyqyaify.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.zdbjq.cn/Article/details/gxhmkrnga.sHtML


<!-- 参考信息 -->