代发 wailian999

esac
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpysvqfot.sHtML

[R12] for 遍历文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdynovhv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gjmffexup.sHtML

[R13] for 计数循环
来源：http://blog.fanxiaobao.xyz/Article/details/gunnslvsz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gfaykckzb.sHtML

[R14] C 风格 for
来源：http://3g.fanxiaobao.xyz/Article/details/gkbdgmfzo.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxguegykh.sHtML

[R15] while 逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gdymkuyqh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gtjdkzjnj.sHtML

[R16] until 等待条件
来源：http://baike.fanxiaobao.xyz/Article/details/gwhvphhhh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gdydvmhqt.sHtML

[R17] 数组定义与取值
来源：http://wap.fanxiaobao.xyz/Article/details/gmzuxrhpb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gwntqubhh.sHtML

[R18] 遍历数组
来源：http://blog.fanxiaobao.xyz/Article/details/ggkyhbhjw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghqunfzzt.sHtML

[R19] 数组长度
来源：http://baike.fanxiaobao.xyz/Article/details/ghrffgmwf.sHtML

echo "${#arr[@]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gvsfhcyga.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fanxiaobao.xyz/Article/details/gizkpfwot.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gisddrqev.sHtML

[R21] 字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/grskhnvek.sHtML

echo "${#s}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxaksprqd.sHtML

[R22] 截取子串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbyvmcli.sHtML

echo "${s:0:5}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gfqhzipov.sHtML

[R23] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnkdmzgvv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fanxiaobao.xyz/Article/details/guovhmpsl.sHtML

[R24] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gauzwlpzg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fanxiaobao.xyz/Article/details/gsaydgzrc.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsbaoobof.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxrnvejn.sHtML

[R26] 命令替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gcidibkqd.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gngoadycd.sHtML

[R27] 算术展开
来源：http://mobile.fanxiaobao.xyz/Article/details/gdkwypuoy.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fanxiaobao.xyz/Article/details/grevmluyz.sHtML

[R28] 浮点运算
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbzpoejni.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fanxiaobao.xyz/Article/details/gkbcqdtzc.sHtML

[R29] 定义函数
来源：http://mobile.fanxiaobao.xyz/Article/details/ggbvzkanf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvhrlisjj.sHtML

[R30] 函数返回状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gnwjionqa.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fanxiaobao.xyz/Article/details/gynbvecmt.sHtML

[R31] 局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gicoyihkh.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gomptjbjo.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzblrrisq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdwlxmdsf.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fanxiaobao.xyz/Article/details/gbpwunyam.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzchjegsq.sHtML

[R34] 退出时清理
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggvuyqckg.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gbtppujfj.sHtML

[R35] 后台执行并等待
来源：http://3g.fanxiaobao.xyz/Article/details/gddlgrpix.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fanxiaobao.xyz/Article/details/gfnjlijrc.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gplnozfze.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fanxiaobao.xyz/Article/details/gcoigjpxc.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebqzbvvs.sHtML

files=$(ls -1)
来源：http://baike.fanxiaobao.xyz/Article/details/gkqrnrolo.sHtML

[R38] 管道串联
来源：http://m.share.fanxiaobao.xyz/Article/details/gluhqxceb.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fanxiaobao.xyz/Article/details/gyhqwrain.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjxhwzzv.sHtML

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gfjbrvmvc.sHtML

[R40] 追加写日志
来源：http://baike.fanxiaobao.xyz/Article/details/gtcirulwg.sHtML

echo "log" >> out.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gjauaognf.sHtML

[R41] 丢弃输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjmpsvbvg.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gakjftrmj.sHtML

[R42] 输入重定向
来源：http://wap.fanxiaobao.xyz/Article/details/gfeoruste.sHtML

wc -l < a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gfysnezdf.sHtML

[R43] 按名字查找文件
来源：http://blog.fanxiaobao.xyz/Article/details/gevkaxrmm.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/grkqwtkxu.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxurnyyyy.sHtML

find . -mtime -7 -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gsqdfuzkr.sHtML

[R45] 批量删除
来源：http://mobile.fanxiaobao.xyz/Article/details/ganodboqu.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giuvarwfm.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fanxiaobao.xyz/Article/details/gbnkfxnig.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fanxiaobao.xyz/Article/details/gjwneflpg.sHtML

[R47] sed 单行替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmzaycguv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gevifwvxo.sHtML

[R48] awk 取指定列
来源：http://baike.fanxiaobao.xyz/Article/details/gfngwupus.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gdeyicngt.sHtML

[R49] awk 带条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsnavinlx.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fanxiaobao.xyz/Article/details/gijzlgpkh.sHtML

[R50] awk 求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gcbptugjy.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gdeigcvvs.sHtML

[R51] 排序去重取前几
来源：http://mobile.fanxiaobao.xyz/Article/details/gqlztpbrg.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fanxiaobao.xyz/Article/details/gotznznub.sHtML

[R52] 统计行数
来源：http://www.share.fanxiaobao.xyz/Article/details/gderzfcod.sHtML

wc -l a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/giyzbqrtv.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fanxiaobao.xyz/Article/details/gzjxqhunq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gqfezepuq.sHtML

[R54] 比较两个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gzsnudrso.sHtML

diff a.txt b.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gjwasnyrd.sHtML

[R55] 压缩与解压
来源：http://m.share.fanxiaobao.xyz/Article/details/gfxtkbvsh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkvzxsesp.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcittifwa.sHtML

scp file user@host:/path/
来源：http://blog.fanxiaobao.xyz/Article/details/gonbwkvoy.sHtML

[R57] 远程执行命令
来源：http://baike.fanxiaobao.xyz/Article/details/gknwcflxk.sHtML

ssh user@host 'uptime'
来源：http://3g.fanxiaobao.xyz/Article/details/gaanjashw.sHtML

[R58] 下载文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gelcyoadg.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fanxiaobao.xyz/Article/details/goivgzctr.sHtML

[R59] 发 POST JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gxlnxqlnt.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glchqsusf.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxutymexz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gppqaqpit.sHtML

[R61] 磁盘占用
来源：http://3g.fanxiaobao.xyz/Article/details/gdsxclfyn.sHtML

df -h;  du -sh *
来源：http://www.share.fanxiaobao.xyz/Article/details/ghymvnphk.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gnnbfbupl.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjpwmmpqh.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/guhazhzam.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fanxiaobao.xyz/Article/details/ghdffxgwu.sHtML

[R64] 结束进程
来源：http://3g.fanxiaobao.xyz/Article/details/gahbbpcwu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghlwauzhq.sHtML

[R65] 查看端口占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gckbbznnj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fanxiaobao.xyz/Article/details/gahhfgwtb.sHtML

[R66] 定时任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwqvzymdk.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaqimozoz.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fanxiaobao.xyz/Article/details/ghcjyxukg.sHtML

openssl rand -hex 16
来源：http://www.blog.fanxiaobao.xyz/Article/details/gskkppbcb.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsongljwc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/guhcwbyoh.sHtML

[R69] 生成随机密码
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxaotvvi.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fanxiaobao.xyz/Article/details/gaaoqgkwp.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gybflksyf.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fanxiaobao.xyz/Article/details/ggqpvnefg.sHtML

[R71] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gxslgwdbr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fanxiaobao.xyz/Article/details/ghgtbjigy.sHtML

[R72] 等待端口就绪
来源：http://baike.fanxiaobao.xyz/Article/details/gefohmhpk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gzddsuhki.sHtML

[R73] 分割大日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gmdaloykn.sHtML

split -l 1000 big.log part_
来源：http://wap.fanxiaobao.xyz/Article/details/goatabjci.sHtML

[R74] 批量重命名
来源：http://baike.fanxiaobao.xyz/Article/details/gvitldbsu.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/glvkddfum.sHtML

[R75] 导出环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gmwbmjzfa.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/gzvdootwh.sHtML

[R76] 使用临时文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gppeaofge.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gibxigtky.sHtML

[R77] 读取用户输入
来源：http://blog.fanxiaobao.xyz/Article/details/gwkgpmrvb.sHtML

read -rp "请输入: " ans
来源：http://3g.fanxiaobao.xyz/Article/details/gowrqgcmj.sHtML

[R78] 交互式菜单
来源：http://3g.fanxiaobao.xyz/Article/details/gnujflvlc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwzjgdaq.sHtML

[R79] 解析命令行选项
来源：http://baike.fanxiaobao.xyz/Article/details/grdpqouuc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdgpeaeeq.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/goqrxwcne.sHtML

time ./run.sh
来源：http://www.share.fanxiaobao.xyz/Article/details/gdjjgcgxk.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbbsmbux.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gwqizpelj.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/galytihdd.sHtML

[S01] C：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gvzayrdhf.sHtML

#include <stdio.h>
来源：http://blog.fanxiaobao.xyz/Article/details/gfifledsf.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmlcrrpk.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fanxiaobao.xyz/Article/details/gftyxiwad.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqkfdcpee.sHtML

[S03] C：读入整数
来源：http://www.share.fanxiaobao.xyz/Article/details/ggmsrxtmg.sHtML

int x; scanf("%d", &x);
来源：http://wap.fanxiaobao.xyz/Article/details/gawwqvqgu.sHtML

[S04] C：字符串复制
来源：http://www.share.fanxiaobao.xyz/Article/details/gyqzcqmlx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fanxiaobao.xyz/Article/details/gmjfqnsxi.sHtML

[S05] C：字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmxhlkost.sHtML

strlen(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdoxijwsw.sHtML

[S06] C：字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjdpifek.sHtML

strcmp(a, b) == 0
来源：http://www.share.fanxiaobao.xyz/Article/details/gessnfhxh.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdceawux.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fanxiaobao.xyz/Article/details/geiswjlzf.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhikzreu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fanxiaobao.xyz/Article/details/gbfjkzymi.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fanxiaobao.xyz/Article/details/ghlfsgcaj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fanxiaobao.xyz/Article/details/gkkmqewjd.sHtML

[S10] C：指针与解引用
来源：http://read.share.fanxiaobao.xyz/Article/details/gjiiztqvt.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcsmkitcm.sHtML

[S11] C：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gliqowtai.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/gfazpbkoz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcxedbvvd.sHtML

fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gopbhruim.sHtML

[S12] C：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/glnbyobby.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhaekqwa.sHtML

[S13] C：宏定义
来源：http://blog.fanxiaobao.xyz/Article/details/gflxyojdf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fanxiaobao.xyz/Article/details/gewzctdfk.sHtML

[S14] C：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gbgwwcpfn.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fanxiaobao.xyz/Article/details/ghijxerwx.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gjplorpgv.sHtML

(double) a / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gcjculjik.sHtML

[S16] C：位操作置位
来源：http://blog.fanxiaobao.xyz/Article/details/glccmably.sHtML

x |= (1 << 3);
来源：http://blog.fanxiaobao.xyz/Article/details/giopeasfd.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gnuladuqn.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fanxiaobao.xyz/Article/details/gpbjiwltn.sHtML

[S18] C：命令行参数
来源：http://m.share.fanxiaobao.xyz/Article/details/ghixspqwn.sHtML

int main(int argc, char **argv)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpnkjouyl.sHtML

[S19] C：快速排序
来源：http://baike.fanxiaobao.xyz/Article/details/gmmdqkrpn.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gsunhdjev.sHtML

[S20] C：二分查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gfrgokpfe.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gbbykdtpl.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/gxflczxzb.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fanxiaobao.xyz/Article/details/gwspfklnm.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/guikzlhuq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fanxiaobao.xyz/Article/details/gwpulkmoh.sHtML

[S23] C：随机数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpfdsosls.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gvnorwgys.sHtML

[S24] C：获取本地时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gmxcxdrvf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gctwnrpez.sHtML

[S25] C：内存拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/guxqhhpyx.sHtML

memcpy(dst, src, n);
来源：http://read.share.fanxiaobao.xyz/Article/details/gneyleetq.sHtML

[S26] C：内存清零
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmzspuvi.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fanxiaobao.xyz/Article/details/gxsazjxtz.sHtML

[S27] C：定义常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gavnmnvfh.sHtML

const double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtpsfstvq.sHtML

[S28] C：静态变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gmvoifoos.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gooupphsf.sHtML

[S29] C：变参函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gweehgykv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqsaluqq.sHtML

[S30] C：头文件保护
来源：http://mobile.fanxiaobao.xyz/Article/details/ggeycbvva.sHtML

#ifndef X_H
来源：http://baike.fanxiaobao.xyz/Article/details/gwnqfmeqi.sHtML

#define X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfdpsposg.sHtML

#endif
来源：http://blog.fanxiaobao.xyz/Article/details/gikrbunll.sHtML

[S31] C++：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/guajvywgk.sHtML

#include <iostream>
来源：http://wap.fanxiaobao.xyz/Article/details/gsccwxbkc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gduuekamr.sHtML

[S32] C++：字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gvxzmsopu.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fanxiaobao.xyz/Article/details/guxjsckfm.sHtML

[S33] C++：vector 增删
来源：http://m.share.fanxiaobao.xyz/Article/details/gzbybkixt.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfulaohlj.sHtML

[S34] C++：遍历 vector
来源：http://3g.fanxiaobao.xyz/Article/details/goyszopbk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gvodadwwd.sHtML

[S35] C++：map
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggkuditjb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/grmdoakyt.sHtML

[S36] C++：unordered_map
来源：http://blog.fanxiaobao.xyz/Article/details/gejjsmfcb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/googlljpg.sHtML

[S37] C++：set
来源：http://baike.fanxiaobao.xyz/Article/details/glskwoysv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gkhokxgsk.sHtML

[S38] C++：排序
来源：http://wap.fanxiaobao.xyz/Article/details/gqewbjpuh.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/ghljgmxrt.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fanxiaobao.xyz/Article/details/gciipacti.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fanxiaobao.xyz/Article/details/gvorvjzle.sHtML

[S40] C++：查找元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gknaayjcy.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwwubelzw.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fanxiaobao.xyz/Article/details/ghfpkmecq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fanxiaobao.xyz/Article/details/gpsmvvjtf.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpwowwvqt.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fanxiaobao.xyz/Article/details/gpraqrlos.sHtML

[S43] C++：智能指针
来源：http://www.share.fanxiaobao.xyz/Article/details/gtnaexfrw.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbzqzowzk.sHtML

[S44] C++：引用传参
来源：http://read.share.fanxiaobao.xyz/Article/details/gjyyvbjku.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdfcdaghu.sHtML

[S45] C++：lambda
来源：http://3g.fanxiaobao.xyz/Article/details/gbcfhrehq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gszxbvidt.sHtML

[S46] C++：函数模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gasgcnpbv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqegmynqd.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gkzhkjtas.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fanxiaobao.xyz/Article/details/grgcrzgjb.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gflaoqhip.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fanxiaobao.xyz/Article/details/glowevsud.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gpsmkurin.sHtML

[S49] C++：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gcvpoemco.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/gyyuqavwb.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjysitce.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqjqdsefu.sHtML

[S51] C++：显式类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gxrtgzhwc.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbnziymsk.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fanxiaobao.xyz/Article/details/gkoxmzezi.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fanxiaobao.xyz/Article/details/gvayzkmdu.sHtML

[S53] C++：移动语义
来源：http://m.share.fanxiaobao.xyz/Article/details/geltummzp.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggojcmqvq.sHtML

[S54] C++：异常处理
来源：http://baike.fanxiaobao.xyz/Article/details/gvkvlhpgr.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmnsmgml.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/ghcqlivdj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fanxiaobao.xyz/Article/details/gzebzlvyj.sHtML

[S56] C++：optional
来源：http://wap.fanxiaobao.xyz/Article/details/gcyvmnkso.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gttygtzlv.sHtML

[S57] C++：编译期常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gnsdpsuzu.sHtML

constexpr int N = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/ggxbnwyqj.sHtML

[S58] C++：命名空间
来源：http://m.share.fanxiaobao.xyz/Article/details/gysrlmzfi.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnmoipihb.sHtML

[S59] C++：静态断言
来源：http://wap.fanxiaobao.xyz/Article/details/gdnguuygi.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fanxiaobao.xyz/Article/details/gmrtuiwif.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fanxiaobao.xyz/Article/details/gwyiwljto.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/geeosagmf.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/grcdrppbz.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fanxiaobao.xyz/Article/details/gzutbdvrx.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzuojdlkm.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfpsqebnc.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gwostgmzb.sHtML

[T02] Kotlin：变量
来源：http://blog.fanxiaobao.xyz/Article/details/gznujfteo.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fanxiaobao.xyz/Article/details/gyrfipvky.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fanxiaobao.xyz/Article/details/gqkipesmx.sHtML

"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvsjxdnf.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gygequpol.sHtML

val n: String? = null;  n?.length
来源：http://blog.fanxiaobao.xyz/Article/details/gmbtjilwt.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gqlbeynhs.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fanxiaobao.xyz/Article/details/gpfgfpizm.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/gznqcgpli.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjsmncyxo.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gqeiycgtk.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gobsjnkwu.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fanxiaobao.xyz/Article/details/gvkknxiew.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcqkbffgm.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gyojhonsb.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gntshabem.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fanxiaobao.xyz/Article/details/gonnhglan.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fanxiaobao.xyz/Article/details/giirssjww.sHtML

[T11] Kotlin：协程
来源：http://3g.fanxiaobao.xyz/Article/details/gevjhdqph.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjlomghpw.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fanxiaobao.xyz/Article/details/gnxktneim.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghajykbfe.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fanxiaobao.xyz/Article/details/gtozydtek.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gracohzfx.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gymkeqhyw.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gydobdryx.sHtML


<!-- 参考信息 -->