代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gtnjqsbui.sHtML

[R14] C 风格 for
来源：http://mobile.fanxiaobao.xyz/Article/details/gtgbexjmn.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gsqeminnn.sHtML

[R15] while 逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gdkfmutgs.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbsietnnm.sHtML

[R16] until 等待条件
来源：http://3g.fanxiaobao.xyz/Article/details/gmchxcwhp.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gmdfzeeiw.sHtML

[R17] 数组定义与取值
来源：http://wap.fanxiaobao.xyz/Article/details/guqrvrjep.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gfgvwljhn.sHtML

[R18] 遍历数组
来源：http://blog.fanxiaobao.xyz/Article/details/gswkmddxx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gejjqvdie.sHtML

[R19] 数组长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gecukqond.sHtML

echo "${#arr[@]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gpebhzrir.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fanxiaobao.xyz/Article/details/gkeguzdjk.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gubquevmd.sHtML

[R21] 字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gcbtwcilr.sHtML

echo "${#s}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyfrhmwdo.sHtML

[R22] 截取子串
来源：http://baike.fanxiaobao.xyz/Article/details/gzdataifw.sHtML

echo "${s:0:5}"
来源：http://3g.fanxiaobao.xyz/Article/details/gskawhzgz.sHtML

[R23] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gavpbzbof.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fanxiaobao.xyz/Article/details/grxrdiros.sHtML

[R24] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/grlwsuxeg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/gaabnjsok.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/gqramcagm.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fanxiaobao.xyz/Article/details/gkidzthfn.sHtML

[R26] 命令替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gxrdxyvlr.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guhktmgdd.sHtML

[R27] 算术展开
来源：http://blog.fanxiaobao.xyz/Article/details/gdxlktoti.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzvgsosla.sHtML

[R28] 浮点运算
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcvauzvgb.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwxwpppnf.sHtML

[R29] 定义函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggwcmbpbq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqbaxryz.sHtML

[R30] 函数返回状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gttyptmza.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fanxiaobao.xyz/Article/details/gzhxrjhwa.sHtML

[R31] 局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gsykfufkw.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gtlcygqwd.sHtML

[R32] 参数个数校验
来源：http://blog.fanxiaobao.xyz/Article/details/gxktpssvq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdwqdbsgx.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/givmznrxt.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fanxiaobao.xyz/Article/details/gmevjkaxv.sHtML

[R34] 退出时清理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmzrhmdmq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gercsoxgu.sHtML

[R35] 后台执行并等待
来源：http://blog.fanxiaobao.xyz/Article/details/glqzlhufs.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fanxiaobao.xyz/Article/details/gplgyegyj.sHtML

[R36] 并发执行多个任务
来源：http://3g.fanxiaobao.xyz/Article/details/gfixzajhk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fanxiaobao.xyz/Article/details/grswzwwjh.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gtrrvmbfm.sHtML

files=$(ls -1)
来源：http://blog.fanxiaobao.xyz/Article/details/gzpzojnbh.sHtML

[R38] 管道串联
来源：http://3g.fanxiaobao.xyz/Article/details/gppudyhrl.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fanxiaobao.xyz/Article/details/gjnjbxgrf.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmatkthex.sHtML

cmd > out.log 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gfpnkrukr.sHtML

[R40] 追加写日志
来源：http://baike.fanxiaobao.xyz/Article/details/guxcprejd.sHtML

echo "log" >> out.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gbuggwsdo.sHtML

[R41] 丢弃输出
来源：http://www.share.fanxiaobao.xyz/Article/details/grqzahfio.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gnpvtpeiw.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/ghoejrtrx.sHtML

wc -l < a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grbmzixbn.sHtML

[R43] 按名字查找文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gqoekhhoe.sHtML

find . -name "*.log" -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gqiwpxukj.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqiloqajt.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/ggepesktj.sHtML

[R45] 批量删除
来源：http://baike.fanxiaobao.xyz/Article/details/ghrsjvzla.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fanxiaobao.xyz/Article/details/gqosesadm.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpfnpswwe.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/gbmxmxcec.sHtML

[R47] sed 单行替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gcxzlojnm.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwajcqmhr.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grmipoprp.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gpbwiawct.sHtML

[R49] awk 带条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gvwintwqv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fanxiaobao.xyz/Article/details/gzesljwmm.sHtML

[R50] awk 求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gvusyoese.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/ghrtrqdki.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkcfmolqk.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fanxiaobao.xyz/Article/details/gywllrrrm.sHtML

[R52] 统计行数
来源：http://wap.fanxiaobao.xyz/Article/details/gykxtzvjp.sHtML

wc -l a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/geiielrcg.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fanxiaobao.xyz/Article/details/gfussrvdn.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gsonmtffz.sHtML

[R54] 比较两个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/geesozfqq.sHtML

diff a.txt b.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gbrzrtgwv.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/gfsnvtjcj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fanxiaobao.xyz/Article/details/gcbysoomc.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ganbqunaq.sHtML

scp file user@host:/path/
来源：http://3g.fanxiaobao.xyz/Article/details/gzeyeecxw.sHtML

[R57] 远程执行命令
来源：http://blog.fanxiaobao.xyz/Article/details/ghhkvrhdn.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/golnxllcy.sHtML

[R58] 下载文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gwdxkuxyc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fanxiaobao.xyz/Article/details/gkyshdrvk.sHtML

[R59] 发 POST JSON
来源：http://3g.fanxiaobao.xyz/Article/details/gmhviclay.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fanxiaobao.xyz/Article/details/ggutpkrdv.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fanxiaobao.xyz/Article/details/ghuscdbhn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfmmjdiil.sHtML

[R61] 磁盘占用
来源：http://wap.fanxiaobao.xyz/Article/details/gpmnvrsup.sHtML

df -h;  du -sh *
来源：http://mobile.fanxiaobao.xyz/Article/details/gshdoojvh.sHtML

[R62] 找最占空间的文件
来源：http://blog.fanxiaobao.xyz/Article/details/glxetpmmh.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcpupgcgn.sHtML

[R63] 内存与进程
来源：http://baike.fanxiaobao.xyz/Article/details/gmgbvigxb.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fanxiaobao.xyz/Article/details/gfcfspsad.sHtML

[R64] 结束进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gqnzcadno.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhbysvht.sHtML

[R65] 查看端口占用
来源：http://3g.fanxiaobao.xyz/Article/details/gwaammnta.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fanxiaobao.xyz/Article/details/gahlkrulz.sHtML

[R66] 定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gzbtkwnpy.sHtML

crontab -e;  crontab -l
来源：http://baike.fanxiaobao.xyz/Article/details/gjhkznxry.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fanxiaobao.xyz/Article/details/grfovspar.sHtML

openssl rand -hex 16
来源：http://mobile.fanxiaobao.xyz/Article/details/gsbuelkuc.sHtML

[R68] 计算文件校验值
来源：http://mobile.fanxiaobao.xyz/Article/details/gyeiuzdvk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gohyrxqng.sHtML

[R69] 生成随机密码
来源：http://read.share.fanxiaobao.xyz/Article/details/govzwoxjh.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/gzwxpwzgm.sHtML

[R70] 时间戳与互转
来源：http://3g.fanxiaobao.xyz/Article/details/ghpccsolr.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fanxiaobao.xyz/Article/details/gyadsiczt.sHtML

[R71] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gqqiryarr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fanxiaobao.xyz/Article/details/gltfynfrh.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/gghtbkdif.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gumolppkp.sHtML

[R73] 分割大日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gscfeckty.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fanxiaobao.xyz/Article/details/gppknepyw.sHtML

[R74] 批量重命名
来源：http://wap.fanxiaobao.xyz/Article/details/ggurdwfqr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gtyvbhccw.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqrkislcd.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fanxiaobao.xyz/Article/details/gkgqttfvf.sHtML

[R76] 使用临时文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvdegoed.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtwoxthwx.sHtML

[R77] 读取用户输入
来源：http://www.share.fanxiaobao.xyz/Article/details/glrbkdywb.sHtML

read -rp "请输入: " ans
来源：http://3g.fanxiaobao.xyz/Article/details/glhkrcqvl.sHtML

[R78] 交互式菜单
来源：http://wap.fanxiaobao.xyz/Article/details/gcttwwwvn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gixuwwmbu.sHtML

[R79] 解析命令行选项
来源：http://www.share.fanxiaobao.xyz/Article/details/gepqnizzw.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gyytsloyh.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fanxiaobao.xyz/Article/details/gwpbiznov.sHtML

time ./run.sh
来源：http://www.share.fanxiaobao.xyz/Article/details/gegnvfhnm.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gdifonupm.sHtML

S. C / C++ 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtlimztpz.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grkillnby.sHtML

[S01] C：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gulohhssh.sHtML

#include <stdio.h>
来源：http://blog.fanxiaobao.xyz/Article/details/gzywsvmra.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghnlvfaxd.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gzzpssqpj.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gajfedoqc.sHtML

[S03] C：读入整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqicceuer.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjfitxxlj.sHtML

[S04] C：字符串复制
来源：http://3g.fanxiaobao.xyz/Article/details/geoldmgyd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/grbeafiud.sHtML

[S05] C：字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gtrybnjoi.sHtML

strlen(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/golbogyzf.sHtML

[S06] C：字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gnligkieo.sHtML

strcmp(a, b) == 0
来源：http://www.share.fanxiaobao.xyz/Article/details/gzoyncjfx.sHtML

[S07] C：数组遍历求和
来源：http://baike.fanxiaobao.xyz/Article/details/gkgvojqoq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fanxiaobao.xyz/Article/details/goluekomp.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fanxiaobao.xyz/Article/details/gpdavlagj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdfunfsth.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fanxiaobao.xyz/Article/details/gcaqflzoy.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fanxiaobao.xyz/Article/details/gxbxgecyb.sHtML

[S10] C：指针与解引用
来源：http://www.share.fanxiaobao.xyz/Article/details/ghpoesmax.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/gerngyign.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glrakibwl.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fanxiaobao.xyz/Article/details/gflpxaeil.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gttdrwbzs.sHtML

fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gfcbmdmqn.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gomxjsxgv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmbcbyfnr.sHtML

[S13] C：宏定义
来源：http://blog.fanxiaobao.xyz/Article/details/gtqjcpuwp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqvrqlxqp.sHtML

[S14] C：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gsuhxhord.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fanxiaobao.xyz/Article/details/gfzxmkaad.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmkdqedgk.sHtML

(double) a / b
来源：http://read.share.fanxiaobao.xyz/Article/details/ggdkccpdl.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gexmgoebd.sHtML

x |= (1 << 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gpgimsltt.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gigzhdchf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpvvejyiy.sHtML

[S18] C：命令行参数
来源：http://m.share.fanxiaobao.xyz/Article/details/ggpbvqyqe.sHtML

int main(int argc, char **argv)
来源：http://3g.fanxiaobao.xyz/Article/details/gyssrjehq.sHtML

[S19] C：快速排序
来源：http://3g.fanxiaobao.xyz/Article/details/gynmpigkj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/grqbierzn.sHtML

[S20] C：二分查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gzkqxknvi.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gwgwobmfe.sHtML

[S21] C：字符类别判断
来源：http://baike.fanxiaobao.xyz/Article/details/glzhorvqc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fanxiaobao.xyz/Article/details/gcmcuyxmn.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glrcocehk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/gqijlholz.sHtML

[S23] C：随机数
来源：http://wap.fanxiaobao.xyz/Article/details/gyoqlyvby.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggdyxqfqv.sHtML

[S24] C：获取本地时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gpqjbeesu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fanxiaobao.xyz/Article/details/glqgehvev.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzdcflxlx.sHtML

memcpy(dst, src, n);
来源：http://mobile.fanxiaobao.xyz/Article/details/gezmralsy.sHtML

[S26] C：内存清零
来源：http://read.share.fanxiaobao.xyz/Article/details/gznvetbto.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggdqxcajy.sHtML

[S27] C：定义常量
来源：http://baike.fanxiaobao.xyz/Article/details/gyqouvbed.sHtML

const double PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/glebyunvw.sHtML

[S28] C：静态变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gginlbeye.sHtML

static int counter = 0;
来源：http://www.share.fanxiaobao.xyz/Article/details/grrnhyztg.sHtML

[S29] C：变参函数
来源：http://3g.fanxiaobao.xyz/Article/details/gddimgfks.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwbfmivlx.sHtML

[S30] C：头文件保护
来源：http://mobile.fanxiaobao.xyz/Article/details/gfgyhnrsp.sHtML

#ifndef X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gqdtxhixe.sHtML

#define X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gujqclody.sHtML

#endif
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxjvgitu.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glbcxyhtr.sHtML

#include <iostream>
来源：http://baike.fanxiaobao.xyz/Article/details/gozazzzfd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmxjmzsei.sHtML

[S32] C++：字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfdmkpgqc.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fanxiaobao.xyz/Article/details/gmugemmci.sHtML

[S33] C++：vector 增删
来源：http://read.share.fanxiaobao.xyz/Article/details/gxpilkvbt.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjksngkap.sHtML

[S34] C++：遍历 vector
来源：http://wap.fanxiaobao.xyz/Article/details/glrgqxzsl.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdcfjdrjr.sHtML

[S35] C++：map
来源：http://mobile.fanxiaobao.xyz/Article/details/gjtsyzaml.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grgjfaiyl.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkdwnjhrp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gskitosyf.sHtML

[S37] C++：set
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmzqzecxg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gejzhgntx.sHtML

[S38] C++：排序
来源：http://m.share.fanxiaobao.xyz/Article/details/ggstlkdjz.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gesqzysgz.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gujwhmxap.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fanxiaobao.xyz/Article/details/getwfeihr.sHtML

[S40] C++：查找元素
来源：http://mobile.fanxiaobao.xyz/Article/details/galhaoyre.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fanxiaobao.xyz/Article/details/ghvsafttc.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gtuwcaayg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gsquijrks.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fanxiaobao.xyz/Article/details/gjckdenfn.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fanxiaobao.xyz/Article/details/gvbkqbydi.sHtML

[S43] C++：智能指针
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkmeippkr.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkipjobra.sHtML

[S44] C++：引用传参
来源：http://m.share.fanxiaobao.xyz/Article/details/gjencyhqr.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grvuvmjik.sHtML

[S45] C++：lambda
来源：http://3g.fanxiaobao.xyz/Article/details/gdcqynnme.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fanxiaobao.xyz/Article/details/gmhrszgvu.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmwgflwtr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gplfwlcjc.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gfkcanuus.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fanxiaobao.xyz/Article/details/gclnejdui.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdefzlsvh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpayifulb.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqpywvpao.sHtML

[S49] C++：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geonpoiqm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwvulkoes.sHtML

[S50] C++：格式化数字
来源：http://baike.fanxiaobao.xyz/Article/details/gpxbaxzlg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwaqvbruv.sHtML

[S51] C++：显式类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gfbkkqpth.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glhtvdbvw.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fanxiaobao.xyz/Article/details/gpaytllgg.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fanxiaobao.xyz/Article/details/gfpmufcld.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzrfujtkd.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fanxiaobao.xyz/Article/details/gkubyhxxa.sHtML

[S54] C++：异常处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gkfcxiucx.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gahsrsxbd.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpmttmifv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fanxiaobao.xyz/Article/details/gnrtoxrwy.sHtML

[S56] C++：optional
来源：http://www.share.fanxiaobao.xyz/Article/details/ggesvmklm.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fanxiaobao.xyz/Article/details/gxoulriex.sHtML

[S57] C++：编译期常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gnuspodme.sHtML

constexpr int N = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gufpfmoxb.sHtML

[S58] C++：命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/gphmkpxic.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gptrgakyy.sHtML

[S59] C++：静态断言
来源：http://www.share.fanxiaobao.xyz/Article/details/gtmhkqxop.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhnhqjmj.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwoatwcfa.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/ggftbikme.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gkllxoaan.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fanxiaobao.xyz/Article/details/gicztcbmb.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gahpgjltr.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gjbujmxig.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gqwvukojy.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsktwldlx.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fanxiaobao.xyz/Article/details/gpcvboeeq.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fanxiaobao.xyz/Article/details/gnktnnlgh.sHtML

"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gdfaltwfk.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghwpdaigs.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gemfgjjjn.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gtbhsrfts.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fanxiaobao.xyz/Article/details/grtgrcffd.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/gfglwsqun.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gewfpjeie.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gyimyvpcm.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmizubgxm.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fanxiaobao.xyz/Article/details/glflziemx.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzphtvqai.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gjxppahok.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fanxiaobao.xyz/Article/details/gzcfehvyi.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqwjzxmae.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gspbjyrwj.sHtML

[T11] Kotlin：协程
来源：http://mobile.fanxiaobao.xyz/Article/details/garrgxckj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkefpesno.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grzfxybji.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gqlluccln.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fanxiaobao.xyz/Article/details/gzvcrtwyu.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpieiiyfc.sHtML

[T14] Kotlin：循环
来源：http://baike.fanxiaobao.xyz/Article/details/gyheichur.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyedjddgy.sHtML

[T15] Kotlin：接口
来源：http://read.share.fanxiaobao.xyz/Article/details/gmainbibn.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/godyjdppp.sHtML

[T16] Swift：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbufysmo.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwygtdzvu.sHtML


<!-- 参考信息 -->