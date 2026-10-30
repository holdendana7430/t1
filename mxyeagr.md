代发 wailian999

esac
来源：http://m.share.fanxiaobao.xyz/Article/details/gbfilqnti.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcogpqyft.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fanxiaobao.xyz/Article/details/ggtehjqdw.sHtML

[R13] for 计数循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gflgcazfc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxcjnhhr.sHtML

[R14] C 风格 for
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gofxhkamq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/grcsdnkic.sHtML

[R15] while 逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/grybnhjah.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gxjdoyzip.sHtML

[R16] until 等待条件
来源：http://blog.fanxiaobao.xyz/Article/details/gtiaxkreb.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gxgizwzcm.sHtML

[R17] 数组定义与取值
来源：http://blog.fanxiaobao.xyz/Article/details/gvkvjbevt.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gwtvqktwy.sHtML

[R18] 遍历数组
来源：http://blog.fanxiaobao.xyz/Article/details/gllsiazii.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gwmiinohx.sHtML

[R19] 数组长度
来源：http://www.share.fanxiaobao.xyz/Article/details/giietctci.sHtML

echo "${#arr[@]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/goclzgbrg.sHtML

[R20] 关联数组（字典）
来源：http://baike.fanxiaobao.xyz/Article/details/grjhujknd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gxzdwmbjr.sHtML

[R21] 字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gdhciungg.sHtML

echo "${#s}"
来源：http://blog.fanxiaobao.xyz/Article/details/gdvarsjop.sHtML

[R22] 截取子串
来源：http://mobile.fanxiaobao.xyz/Article/details/galzdeiyw.sHtML

echo "${s:0:5}"
来源：http://blog.fanxiaobao.xyz/Article/details/ghwvdbymu.sHtML

[R23] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gbzfbvirw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fanxiaobao.xyz/Article/details/gzvfrkxhy.sHtML

[R24] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glpmvugnd.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fanxiaobao.xyz/Article/details/geualbtzn.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwjzgosq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxbjdfaov.sHtML

[R26] 命令替换
来源：http://3g.fanxiaobao.xyz/Article/details/glnalqopf.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fanxiaobao.xyz/Article/details/gnqxckxoa.sHtML

[R27] 算术展开
来源：http://3g.fanxiaobao.xyz/Article/details/gfxbosbuy.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwueyuvp.sHtML

[R28] 浮点运算
来源：http://wap.fanxiaobao.xyz/Article/details/gszjpbrva.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwlvbjhp.sHtML

[R29] 定义函数
来源：http://wap.fanxiaobao.xyz/Article/details/gdxyocymj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfrgnsqfj.sHtML

[R30] 函数返回状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gbduljxkm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fanxiaobao.xyz/Article/details/gizhhaiex.sHtML

[R31] 局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gxnsesmil.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsuvlkepk.sHtML

[R32] 参数个数校验
来源：http://3g.fanxiaobao.xyz/Article/details/gomhprxwj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzemkobjb.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gvdblaubl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjlkgzxv.sHtML

[R34] 退出时清理
来源：http://www.share.fanxiaobao.xyz/Article/details/ggjvahypr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gekcolnlc.sHtML

[R35] 后台执行并等待
来源：http://mobile.fanxiaobao.xyz/Article/details/gpgekjptx.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fanxiaobao.xyz/Article/details/gojfyscof.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gucmiwmzr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbfvxucqn.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gmswkaobl.sHtML

files=$(ls -1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gptzkprcn.sHtML

[R38] 管道串联
来源：http://www.share.fanxiaobao.xyz/Article/details/gemyvoxtt.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfnkoyxh.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gttojzhhz.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glwqraymf.sHtML

[R40] 追加写日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhrrgsip.sHtML

echo "log" >> out.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmbjxfehd.sHtML

[R41] 丢弃输出
来源：http://read.share.fanxiaobao.xyz/Article/details/goaaazxtz.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gqiltchjz.sHtML

[R42] 输入重定向
来源：http://3g.fanxiaobao.xyz/Article/details/gmylhldie.sHtML

wc -l < a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gmuladtrl.sHtML

[R43] 按名字查找文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gfayhpuyy.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbvxgbxlt.sHtML

[R44] 按修改时间查找
来源：http://wap.fanxiaobao.xyz/Article/details/giinxpqzh.sHtML

find . -mtime -7 -type f
来源：http://blog.fanxiaobao.xyz/Article/details/ggfrfwcfp.sHtML

[R45] 批量删除
来源：http://mobile.fanxiaobao.xyz/Article/details/genfvagje.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fanxiaobao.xyz/Article/details/gpliqzphz.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grygmvoxh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fanxiaobao.xyz/Article/details/guoepydxv.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gymwctmjd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gwaspovqc.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gwwhhkrjw.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/glhufeerg.sHtML

[R49] awk 带条件
来源：http://3g.fanxiaobao.xyz/Article/details/gkcuhfjwd.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fanxiaobao.xyz/Article/details/gsyakansa.sHtML

[R50] awk 求和
来源：http://wap.fanxiaobao.xyz/Article/details/gtzccwokn.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghszsbbak.sHtML

[R51] 排序去重取前几
来源：http://baike.fanxiaobao.xyz/Article/details/gsdtqxqgl.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fanxiaobao.xyz/Article/details/glooibeyj.sHtML

[R52] 统计行数
来源：http://wap.fanxiaobao.xyz/Article/details/gmazkbgqn.sHtML

wc -l a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gystpdrtk.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/gohqwkynk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gayaifdfn.sHtML

[R54] 比较两个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gppkyhlbe.sHtML

diff a.txt b.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gqwgnbfer.sHtML

[R55] 压缩与解压
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfsqrbles.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fanxiaobao.xyz/Article/details/gggekpivk.sHtML

[R56] 远程拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gjxoshbvx.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/gufkvuerp.sHtML

[R57] 远程执行命令
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsfrpdlcm.sHtML

ssh user@host 'uptime'
来源：http://baike.fanxiaobao.xyz/Article/details/gkdyhewfu.sHtML

[R58] 下载文件
来源：http://wap.fanxiaobao.xyz/Article/details/gaukpcaej.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fanxiaobao.xyz/Article/details/geivccoqd.sHtML

[R59] 发 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/gowkbmcmr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fanxiaobao.xyz/Article/details/gtdeiuuix.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gclwipxhc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fanxiaobao.xyz/Article/details/gxbzkutcy.sHtML

[R61] 磁盘占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gbubhexyh.sHtML

df -h;  du -sh *
来源：http://blog.fanxiaobao.xyz/Article/details/gdvskjrmt.sHtML

[R62] 找最占空间的文件
来源：http://baike.fanxiaobao.xyz/Article/details/gcrokmgdn.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fanxiaobao.xyz/Article/details/ghzxedixp.sHtML

[R63] 内存与进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gumbdmgsj.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fanxiaobao.xyz/Article/details/gwluakhac.sHtML

[R64] 结束进程
来源：http://mobile.fanxiaobao.xyz/Article/details/ggbggmjmo.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghesfquoi.sHtML

[R65] 查看端口占用
来源：http://blog.fanxiaobao.xyz/Article/details/grmvmaawv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fanxiaobao.xyz/Article/details/gzlxobxcp.sHtML

[R66] 定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gdodshenz.sHtML

crontab -e;  crontab -l
来源：http://wap.fanxiaobao.xyz/Article/details/gfalqegws.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcjbmljwu.sHtML

openssl rand -hex 16
来源：http://mobile.fanxiaobao.xyz/Article/details/gukulmfyl.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmvnuzovu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gssopurbl.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gttirnjbi.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fanxiaobao.xyz/Article/details/gngcpbfgy.sHtML

[R70] 时间戳与互转
来源：http://3g.fanxiaobao.xyz/Article/details/gjodhhuce.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwvxltbha.sHtML

[R71] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/giwxxmzrv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fanxiaobao.xyz/Article/details/gpocqzwow.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqkrshwed.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gqnhgewxf.sHtML

[R73] 分割大日志
来源：http://blog.fanxiaobao.xyz/Article/details/ghdfpedqc.sHtML

split -l 1000 big.log part_
来源：http://baike.fanxiaobao.xyz/Article/details/gzlycmjze.sHtML

[R74] 批量重命名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gctbnfwsb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwqfmpckn.sHtML

[R75] 导出环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/gqcyyjczh.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fanxiaobao.xyz/Article/details/gqsfcmvpj.sHtML

[R76] 使用临时文件
来源：http://3g.fanxiaobao.xyz/Article/details/gmxfgzhkx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gbjpqlseu.sHtML

[R77] 读取用户输入
来源：http://read.share.fanxiaobao.xyz/Article/details/gqiwnhvky.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fanxiaobao.xyz/Article/details/getonbzyi.sHtML

[R78] 交互式菜单
来源：http://www.blog.fanxiaobao.xyz/Article/details/gggvyymux.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gkzmvuklz.sHtML

[R79] 解析命令行选项
来源：http://wap.fanxiaobao.xyz/Article/details/gbghaiemi.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqiyfhysf.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/gkeoiksbe.sHtML

time ./run.sh
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtxgytqxj.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/grmljaesf.sHtML

S. C / C++ 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/guhncjuxk.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gzggnailm.sHtML

[S01] C：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/ghxnwxlib.sHtML

#include <stdio.h>
来源：http://baike.fanxiaobao.xyz/Article/details/gygwdhwxo.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggtghccch.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fanxiaobao.xyz/Article/details/gxfqmzfcj.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpyrwzzbe.sHtML

[S03] C：读入整数
来源：http://m.share.fanxiaobao.xyz/Article/details/gcyhxbeyt.sHtML

int x; scanf("%d", &x);
来源：http://baike.fanxiaobao.xyz/Article/details/gsampwqnf.sHtML

[S04] C：字符串复制
来源：http://mobile.fanxiaobao.xyz/Article/details/gyukevvsr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/gvdgtusgb.sHtML

[S05] C：字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/guonkoctx.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gengykwst.sHtML

[S06] C：字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gswexuzjd.sHtML

strcmp(a, b) == 0
来源：http://mobile.fanxiaobao.xyz/Article/details/gvaetqbls.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gpgliclkq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpcxjstld.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govcjfftl.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fanxiaobao.xyz/Article/details/gneuxutqq.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fanxiaobao.xyz/Article/details/gzmafruge.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fanxiaobao.xyz/Article/details/gmkrydnjw.sHtML

[S10] C：指针与解引用
来源：http://baike.fanxiaobao.xyz/Article/details/gkacmvfdw.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmxwgtxnt.sHtML

[S11] C：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/grnlcoxpn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsrjclsys.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmvquyjkn.sHtML

fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gerzegtcl.sHtML

[S12] C：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gokeqocav.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggnlhbtbt.sHtML

[S13] C：宏定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbxhbgnkl.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzulobvp.sHtML

[S14] C：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gkiqfyqzm.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqakwcxfl.sHtML

[S15] C：类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gafapjkdm.sHtML

(double) a / b
来源：http://3g.fanxiaobao.xyz/Article/details/gfsunlrsm.sHtML

[S16] C：位操作置位
来源：http://blog.fanxiaobao.xyz/Article/details/gmxrtivev.sHtML

x |= (1 << 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqbdvndzr.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/goncmplmy.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fanxiaobao.xyz/Article/details/gygitvhop.sHtML

[S18] C：命令行参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gkahrisqr.sHtML

int main(int argc, char **argv)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyrsbvgxe.sHtML

[S19] C：快速排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gxvqjwtev.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gfbaaxmgz.sHtML

[S20] C：二分查找
来源：http://baike.fanxiaobao.xyz/Article/details/gbsbcfbob.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxlkcagpw.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshnfyegz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfppthrhe.sHtML

[S22] C：字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gkqqyyvth.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fanxiaobao.xyz/Article/details/gfxjlymwf.sHtML

[S23] C：随机数
来源：http://www.share.fanxiaobao.xyz/Article/details/giubzrlcr.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/glvuqsarm.sHtML

[S24] C：获取本地时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gsnnjxghu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gprqobovn.sHtML

[S25] C：内存拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gtyfkexqe.sHtML

memcpy(dst, src, n);
来源：http://blog.fanxiaobao.xyz/Article/details/ghezumllw.sHtML

[S26] C：内存清零
来源：http://mobile.fanxiaobao.xyz/Article/details/gustlhbuo.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnudtzjgu.sHtML

[S27] C：定义常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmnrenlpv.sHtML

const double PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gxbzjpvap.sHtML

[S28] C：静态变量
来源：http://wap.fanxiaobao.xyz/Article/details/gsgldrwbz.sHtML

static int counter = 0;
来源：http://baike.fanxiaobao.xyz/Article/details/ggbrzqrlj.sHtML

[S29] C：变参函数
来源：http://blog.fanxiaobao.xyz/Article/details/geiphkkjn.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fanxiaobao.xyz/Article/details/gmptowvgx.sHtML

[S30] C：头文件保护
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvbtxjfse.sHtML

#ifndef X_H
来源：http://baike.fanxiaobao.xyz/Article/details/gtxvdwzos.sHtML

#define X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gzobvqubd.sHtML

#endif
来源：http://www.share.fanxiaobao.xyz/Article/details/gfytofsql.sHtML

[S31] C++：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gxskxghma.sHtML

#include <iostream>
来源：http://m.share.fanxiaobao.xyz/Article/details/gqpsuqkcx.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdejfphl.sHtML

[S32] C++：字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gdmzrysiy.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fanxiaobao.xyz/Article/details/gnpfhwclv.sHtML

[S33] C++：vector 增删
来源：http://mobile.fanxiaobao.xyz/Article/details/grkdvyvig.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fanxiaobao.xyz/Article/details/glemfftas.sHtML

[S34] C++：遍历 vector
来源：http://baike.fanxiaobao.xyz/Article/details/gowpblptg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjbjejpq.sHtML

[S35] C++：map
来源：http://mobile.fanxiaobao.xyz/Article/details/grxpvbaec.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gyxwichkn.sHtML

[S36] C++：unordered_map
来源：http://m.share.fanxiaobao.xyz/Article/details/gpcbmlxnn.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gyxfowmmy.sHtML

[S37] C++：set
来源：http://www.share.fanxiaobao.xyz/Article/details/gghkalglp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gbymzqvcx.sHtML

[S38] C++：排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmqemqdxh.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtyperqju.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzpkrzuae.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fanxiaobao.xyz/Article/details/glluclhaq.sHtML

[S40] C++：查找元素
来源：http://www.share.fanxiaobao.xyz/Article/details/griropjzv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gogkrhxvw.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fanxiaobao.xyz/Article/details/grhyipvbu.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gugifpogi.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gmfjutznk.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fanxiaobao.xyz/Article/details/gchngyznw.sHtML

[S43] C++：智能指针
来源：http://www.share.fanxiaobao.xyz/Article/details/gvtpnptpa.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fanxiaobao.xyz/Article/details/gytzvdpla.sHtML

[S44] C++：引用传参
来源：http://mobile.fanxiaobao.xyz/Article/details/gwqbdxjxd.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gthtkfhrw.sHtML

[S45] C++：lambda
来源：http://blog.fanxiaobao.xyz/Article/details/gycufwmdu.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gtsiqcouq.sHtML

[S46] C++：函数模板
来源：http://baike.fanxiaobao.xyz/Article/details/gjfpsggoi.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzpknbuak.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gmagqdnyk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fanxiaobao.xyz/Article/details/gphmmqtiq.sHtML

[S48] C++：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gtgbuxlci.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fanxiaobao.xyz/Article/details/goxbcmoas.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfkjkccax.sHtML

[S49] C++：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gosbakoxg.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fanxiaobao.xyz/Article/details/gdyaoxpvc.sHtML

[S50] C++：格式化数字
来源：http://wap.fanxiaobao.xyz/Article/details/gwivhlscl.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/geiuzdmpj.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/geuckdjgc.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpivxcboj.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fanxiaobao.xyz/Article/details/gmfrhfgwd.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fanxiaobao.xyz/Article/details/gokidwaks.sHtML

[S53] C++：移动语义
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxpqtoew.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtfhdvefr.sHtML

[S54] C++：异常处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gqdbuaccm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gcjkbivdq.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/glbvosdsh.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjwrespoc.sHtML

[S56] C++：optional
来源：http://wap.fanxiaobao.xyz/Article/details/gwikilnzh.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfslhxiub.sHtML

[S57] C++：编译期常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gppvowwxq.sHtML

constexpr int N = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvkikgghr.sHtML

[S58] C++：命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gysyryvss.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtpoglngk.sHtML

[S59] C++：静态断言
来源：http://wap.fanxiaobao.xyz/Article/details/gxctavgtx.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fanxiaobao.xyz/Article/details/gqmpnslcw.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gswokvfgw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/grtjwvctb.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guwpisjco.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fanxiaobao.xyz/Article/details/gbgjatoyg.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gjuzhgeiv.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaewitzbs.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gqnaqqdgl.sHtML

[T02] Kotlin：变量
来源：http://3g.fanxiaobao.xyz/Article/details/gmepmbfpm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fanxiaobao.xyz/Article/details/ghyvqydex.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fanxiaobao.xyz/Article/details/gkgofrfev.sHtML

"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/gojtgnmik.sHtML

[T04] Kotlin：空安全
来源：http://blog.fanxiaobao.xyz/Article/details/gsvotqcwp.sHtML

val n: String? = null;  n?.length
来源：http://wap.fanxiaobao.xyz/Article/details/gyrnenpez.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwtiocfxf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fanxiaobao.xyz/Article/details/gpljvsfoe.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/gkautbsmy.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gqonblwtu.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gpwkuzoqs.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhqfkvpz.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gooxgvtow.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fanxiaobao.xyz/Article/details/grksnnzym.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fanxiaobao.xyz/Article/details/ghvtgxzbv.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fanxiaobao.xyz/Article/details/glslzmkkv.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqyzepgzk.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fanxiaobao.xyz/Article/details/giaowiicz.sHtML

[T11] Kotlin：协程
来源：http://blog.fanxiaobao.xyz/Article/details/gkzohegzy.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdftxwvll.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fanxiaobao.xyz/Article/details/gfpfitjnq.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gstohtuks.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggonzgyby.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gmmcslupv.sHtML

[T14] Kotlin：循环
来源：http://wap.fanxiaobao.xyz/Article/details/ggqvzebwi.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqnlqxoha.sHtML


<!-- 参考信息 -->