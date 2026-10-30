代发 wailian999

esac
来源：http://wap.fanxiaobao.xyz/Article/details/gxedvdpvk.sHtML

[R12] for 遍历文件
来源：http://baike.fanxiaobao.xyz/Article/details/gbrdxacto.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gliknsneg.sHtML

[R13] for 计数循环
来源：http://wap.fanxiaobao.xyz/Article/details/gmxqzjrcy.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gsucwwieb.sHtML

[R14] C 风格 for
来源：http://wap.fanxiaobao.xyz/Article/details/gjpishswz.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gyawxlgdw.sHtML

[R15] while 逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gzludzeup.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gaotsfelv.sHtML

[R16] until 等待条件
来源：http://read.share.fanxiaobao.xyz/Article/details/giwvifjeh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gwenqjjuy.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqasdduhv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gywrhorko.sHtML

[R18] 遍历数组
来源：http://wap.fanxiaobao.xyz/Article/details/gnihstuua.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gcdnnncxg.sHtML

[R19] 数组长度
来源：http://baike.fanxiaobao.xyz/Article/details/gxjevdugc.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtlvbfqwk.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fanxiaobao.xyz/Article/details/grubidqcs.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/geourngiv.sHtML

[R21] 字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzgaqxney.sHtML

echo "${#s}"
来源：http://baike.fanxiaobao.xyz/Article/details/gpbfbydpp.sHtML

[R22] 截取子串
来源：http://baike.fanxiaobao.xyz/Article/details/gxoqdazvv.sHtML

echo "${s:0:5}"
来源：http://m.share.fanxiaobao.xyz/Article/details/glrqvtgtn.sHtML

[R23] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gjpxjyhkf.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnwawgabp.sHtML

[R24] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxdzlvexc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtoftuqle.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/galcgauym.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fanxiaobao.xyz/Article/details/guxeatpxr.sHtML

[R26] 命令替换
来源：http://baike.fanxiaobao.xyz/Article/details/gjygtatdg.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fanxiaobao.xyz/Article/details/gxylxigge.sHtML

[R27] 算术展开
来源：http://wap.fanxiaobao.xyz/Article/details/gwkmvzeex.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/gwjwjqfbf.sHtML

[R28] 浮点运算
来源：http://3g.fanxiaobao.xyz/Article/details/gknizcmgq.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fanxiaobao.xyz/Article/details/giqofdapi.sHtML

[R29] 定义函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gmkerdvyx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gersmlena.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmcdknrx.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fanxiaobao.xyz/Article/details/gfsfezpqa.sHtML

[R31] 局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gznyzpodt.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmdigtkfh.sHtML

[R32] 参数个数校验
来源：http://www.share.fanxiaobao.xyz/Article/details/gfduleywt.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/goscczxsz.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpnadafbf.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkbgaxgpp.sHtML

[R34] 退出时清理
来源：http://wap.fanxiaobao.xyz/Article/details/gckkmhxwp.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gsvxuymne.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fanxiaobao.xyz/Article/details/gddhganwk.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fanxiaobao.xyz/Article/details/gwwpoalwp.sHtML

[R36] 并发执行多个任务
来源：http://blog.fanxiaobao.xyz/Article/details/ghlnihboz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grpyeojlh.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gbctqvhos.sHtML

files=$(ls -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gihnkhleb.sHtML

[R38] 管道串联
来源：http://wap.fanxiaobao.xyz/Article/details/gafmyxryd.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fanxiaobao.xyz/Article/details/gcicdzlsr.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gazoaqgyu.sHtML

cmd > out.log 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmsxkgma.sHtML

[R40] 追加写日志
来源：http://wap.fanxiaobao.xyz/Article/details/gtaooobuw.sHtML

echo "log" >> out.log
来源：http://www.share.fanxiaobao.xyz/Article/details/ghggfuhcz.sHtML

[R41] 丢弃输出
来源：http://blog.fanxiaobao.xyz/Article/details/gxzffghgu.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/goohsjumb.sHtML

[R42] 输入重定向
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwgusknzn.sHtML

wc -l < a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gfalchbuk.sHtML

[R43] 按名字查找文件
来源：http://www.share.fanxiaobao.xyz/Article/details/glpvgvkmg.sHtML

find . -name "*.log" -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gbzsptmir.sHtML

[R44] 按修改时间查找
来源：http://blog.fanxiaobao.xyz/Article/details/gvnipzooc.sHtML

find . -mtime -7 -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gqranjkut.sHtML

[R45] 批量删除
来源：http://www.share.fanxiaobao.xyz/Article/details/gwspfuohk.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjlchwdcl.sHtML

[R46] 递归替换文件内容
来源：http://blog.fanxiaobao.xyz/Article/details/gxkwzluwx.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fanxiaobao.xyz/Article/details/gvhuvvril.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gauqbqwkn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gxqncdxor.sHtML

[R48] awk 取指定列
来源：http://www.blog.fanxiaobao.xyz/Article/details/grugfzdbg.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/garzzzsxy.sHtML

[R49] awk 带条件
来源：http://read.share.fanxiaobao.xyz/Article/details/garfznzby.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fanxiaobao.xyz/Article/details/gtwnvlhbo.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkazzfoxc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/guitkhmrc.sHtML

[R51] 排序去重取前几
来源：http://read.share.fanxiaobao.xyz/Article/details/groyotjzv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fanxiaobao.xyz/Article/details/gnfddssbj.sHtML

[R52] 统计行数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghgxsyyck.sHtML

wc -l a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/giekrooxo.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fanxiaobao.xyz/Article/details/gedrzxhhj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fanxiaobao.xyz/Article/details/gkthhfuef.sHtML

[R54] 比较两个文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gxpdqgqxr.sHtML

diff a.txt b.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gpunucooo.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/giwnwmrbo.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fanxiaobao.xyz/Article/details/gbsvnoikx.sHtML

[R56] 远程拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gdoyckraa.sHtML

scp file user@host:/path/
来源：http://3g.fanxiaobao.xyz/Article/details/gjxbxksmn.sHtML

[R57] 远程执行命令
来源：http://mobile.fanxiaobao.xyz/Article/details/gbnehxzhp.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glxgtxnwg.sHtML

[R58] 下载文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfrjjkmmi.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fanxiaobao.xyz/Article/details/gmvnjtgum.sHtML

[R59] 发 POST JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gcmjisdpc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fanxiaobao.xyz/Article/details/gksnyrddl.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxncffckc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fanxiaobao.xyz/Article/details/gsdwyqkjc.sHtML

[R61] 磁盘占用
来源：http://wap.fanxiaobao.xyz/Article/details/giklnoyog.sHtML

df -h;  du -sh *
来源：http://m.share.fanxiaobao.xyz/Article/details/gavdkbbek.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gjrvdrupj.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqnqmbdqf.sHtML

[R63] 内存与进程
来源：http://3g.fanxiaobao.xyz/Article/details/gfsklygmv.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fanxiaobao.xyz/Article/details/gpuouqjyn.sHtML

[R64] 结束进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gtyrdzocl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fanxiaobao.xyz/Article/details/giadswgfp.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gykyvqchw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghnvzdbek.sHtML

[R66] 定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gkzosrrko.sHtML

crontab -e;  crontab -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gjkdqfahy.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fanxiaobao.xyz/Article/details/gksasywms.sHtML

openssl rand -hex 16
来源：http://blog.fanxiaobao.xyz/Article/details/geesulhvo.sHtML

[R68] 计算文件校验值
来源：http://mobile.fanxiaobao.xyz/Article/details/grbywllqq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gmgluvkmj.sHtML

[R69] 生成随机密码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gieupwbrm.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fanxiaobao.xyz/Article/details/gaygcxtrv.sHtML

[R70] 时间戳与互转
来源：http://mobile.fanxiaobao.xyz/Article/details/gphhxndbc.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/ganmkfutr.sHtML

[R71] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gpmckselg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtrojzxkf.sHtML

[R72] 等待端口就绪
来源：http://blog.fanxiaobao.xyz/Article/details/gryaszfmp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxmmdquq.sHtML

[R73] 分割大日志
来源：http://wap.fanxiaobao.xyz/Article/details/gdkzuzitg.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjkeqwnfz.sHtML

[R74] 批量重命名
来源：http://m.share.fanxiaobao.xyz/Article/details/gqlhzsdhu.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtlmwvftq.sHtML

[R75] 导出环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gczcadvpn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fanxiaobao.xyz/Article/details/grmpufhio.sHtML

[R76] 使用临时文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gyfzovtqt.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gtetwsvkh.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdvnxpluq.sHtML

read -rp "请输入: " ans
来源：http://mobile.fanxiaobao.xyz/Article/details/ghlzszrrw.sHtML

[R78] 交互式菜单
来源：http://baike.fanxiaobao.xyz/Article/details/gjsunffyj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fanxiaobao.xyz/Article/details/gfadtlhwl.sHtML

[R79] 解析命令行选项
来源：http://3g.fanxiaobao.xyz/Article/details/gitwrabzm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gobpqlvok.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmqtbllv.sHtML

time ./run.sh
来源：http://www.share.fanxiaobao.xyz/Article/details/gchbpiayq.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gzfdofobn.sHtML

S. C / C++ 专题
来源：http://3g.fanxiaobao.xyz/Article/details/glexkuile.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gijlyjose.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gdibvtknw.sHtML

#include <stdio.h>
来源：http://wap.fanxiaobao.xyz/Article/details/gtnorphrr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fanxiaobao.xyz/Article/details/gokqztect.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gzaflqakk.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbtiurgql.sHtML

[S03] C：读入整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpgqchncn.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzwlzznqw.sHtML

[S04] C：字符串复制
来源：http://3g.fanxiaobao.xyz/Article/details/gzxrlwwml.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcrybewsn.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gbkhtmmig.sHtML

strlen(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gocmcggpa.sHtML

[S06] C：字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gwopxhfsm.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevmjwbqs.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gjihpmcwp.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fanxiaobao.xyz/Article/details/gjpyebgrg.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fanxiaobao.xyz/Article/details/gvpqfynxs.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfywflzen.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fanxiaobao.xyz/Article/details/gryvdwgvw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fanxiaobao.xyz/Article/details/gvcixvixt.sHtML

[S10] C：指针与解引用
来源：http://blog.fanxiaobao.xyz/Article/details/grijphdhg.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqbiyaalf.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsocdngxr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzgcwncqc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwjohkamu.sHtML

fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzeccfien.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/glgwegqlg.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsqwhkhbe.sHtML

[S13] C：宏定义
来源：http://wap.fanxiaobao.xyz/Article/details/gyeowzkxf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fanxiaobao.xyz/Article/details/glhjrbbvh.sHtML

[S14] C：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/giwrsdvaj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fanxiaobao.xyz/Article/details/gjnrqlsga.sHtML

[S15] C：类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gtasqahar.sHtML

(double) a / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gphszmblj.sHtML

[S16] C：位操作置位
来源：http://3g.fanxiaobao.xyz/Article/details/gvmojuflb.sHtML

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gbcnbdvnl.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gmrclnsyr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fanxiaobao.xyz/Article/details/gejwxiurg.sHtML

[S18] C：命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/gkxkztovb.sHtML

int main(int argc, char **argv)
来源：http://blog.fanxiaobao.xyz/Article/details/gbkxixlza.sHtML

[S19] C：快速排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gnikgeihy.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gcstmnvnw.sHtML

[S20] C：二分查找
来源：http://m.share.fanxiaobao.xyz/Article/details/grzxhtqvt.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gvxdffdxr.sHtML

[S21] C：字符类别判断
来源：http://3g.fanxiaobao.xyz/Article/details/gifgmcptm.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fanxiaobao.xyz/Article/details/gwycxgwuh.sHtML

[S22] C：字符串转数字
来源：http://wap.fanxiaobao.xyz/Article/details/gvideyqvd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/giauyhtmn.sHtML

[S23] C：随机数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goyjxwzxu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnlsgablf.sHtML

[S24] C：获取本地时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gckpdthgn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvgkmwgoe.sHtML

[S25] C：内存拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gyddqocmp.sHtML

memcpy(dst, src, n);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqpxdioae.sHtML

[S26] C：内存清零
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyousxjst.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fanxiaobao.xyz/Article/details/gzsfhqhpm.sHtML

[S27] C：定义常量
来源：http://wap.fanxiaobao.xyz/Article/details/gfutqpquh.sHtML

const double PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gwccvlqan.sHtML

[S28] C：静态变量
来源：http://3g.fanxiaobao.xyz/Article/details/gtxnbjvpk.sHtML

static int counter = 0;
来源：http://blog.fanxiaobao.xyz/Article/details/gvvhmqdkg.sHtML

[S29] C：变参函数
来源：http://3g.fanxiaobao.xyz/Article/details/gefqjfjdp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fanxiaobao.xyz/Article/details/gihvqgzkn.sHtML

[S30] C：头文件保护
来源：http://m.share.fanxiaobao.xyz/Article/details/ggnagqwbd.sHtML

#ifndef X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwifzxhp.sHtML

#define X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gqquerttg.sHtML

#endif
来源：http://wap.fanxiaobao.xyz/Article/details/gzohvdrzw.sHtML

[S31] C++：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gqpugutfr.sHtML

#include <iostream>
来源：http://mobile.fanxiaobao.xyz/Article/details/gbbwlospq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gecqrqeay.sHtML

[S32] C++：字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gazjovylv.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fanxiaobao.xyz/Article/details/gwcrvftur.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fanxiaobao.xyz/Article/details/grkkszknx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvbkluuxi.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fanxiaobao.xyz/Article/details/gakaxmeku.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gcqllophu.sHtML

[S35] C++：map
来源：http://wap.fanxiaobao.xyz/Article/details/gwvsfzkgg.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghnmndwjg.sHtML

[S36] C++：unordered_map
来源：http://www.share.fanxiaobao.xyz/Article/details/gjbjuxqoc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/giuwlqnxq.sHtML

[S37] C++：set
来源：http://m.share.fanxiaobao.xyz/Article/details/giawpissa.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghnjraucf.sHtML

[S38] C++：排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gpcfngwzk.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gczvabhhv.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbmtxfrgk.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fanxiaobao.xyz/Article/details/gtvmqszpd.sHtML

[S40] C++：查找元素
来源：http://3g.fanxiaobao.xyz/Article/details/gzdhwcngs.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gilrqmtay.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fanxiaobao.xyz/Article/details/geomcqvaz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjgeiump.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmaeqhrrk.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fanxiaobao.xyz/Article/details/gjycuxemw.sHtML

[S43] C++：智能指针
来源：http://m.share.fanxiaobao.xyz/Article/details/gdxozyrhn.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzrwlifck.sHtML

[S44] C++：引用传参
来源：http://www.share.fanxiaobao.xyz/Article/details/gkdltvbkq.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpresvirv.sHtML

[S45] C++：lambda
来源：http://baike.fanxiaobao.xyz/Article/details/gunxeykhk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fanxiaobao.xyz/Article/details/ggnioemhq.sHtML

[S46] C++：函数模板
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnzgfodp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fanxiaobao.xyz/Article/details/geqcdtbfn.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/grkxihvhu.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fanxiaobao.xyz/Article/details/gklgrctex.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtwflovrs.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fanxiaobao.xyz/Article/details/gepmcyfcs.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmsevarkj.sHtML

[S49] C++：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gkmbtfmaj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqrrhsgoe.sHtML

[S50] C++：格式化数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gafbrzscc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gyzdcehsn.sHtML

[S51] C++：显式类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gjjevonyk.sHtML

static_cast<double>(a) / b
来源：http://baike.fanxiaobao.xyz/Article/details/gzqjfgdwn.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxgiucclq.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giucpmree.sHtML

[S53] C++：移动语义
来源：http://blog.fanxiaobao.xyz/Article/details/gpjngvasz.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfekqitno.sHtML

[S54] C++：异常处理
来源：http://baike.fanxiaobao.xyz/Article/details/gxkcxnomf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fanxiaobao.xyz/Article/details/glcotnduk.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/glvfispwy.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gopgkndgf.sHtML

[S56] C++：optional
来源：http://mobile.fanxiaobao.xyz/Article/details/gzlywcywz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwrygdunl.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkazngwvv.sHtML

constexpr int N = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gavhylaih.sHtML

[S58] C++：命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpusviltm.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fanxiaobao.xyz/Article/details/gmtuwhtio.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpxbzqiaf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fanxiaobao.xyz/Article/details/ganmsfjyq.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gnthbqeti.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gkybzvmnn.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/geeabtafi.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gexwrjyiz.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqcjjfox.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gdyhopfvi.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gwqwbwzex.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwyeowcgq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fanxiaobao.xyz/Article/details/gtrulfzrw.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gskomebeq.sHtML

"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gumiaoins.sHtML

[T04] Kotlin：空安全
来源：http://baike.fanxiaobao.xyz/Article/details/gyvflhptk.sHtML

val n: String? = null;  n?.length
来源：http://3g.fanxiaobao.xyz/Article/details/gxeclgvzv.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gklwxabtz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fanxiaobao.xyz/Article/details/gdrnsujzs.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fanxiaobao.xyz/Article/details/gngufuxaj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsqmnsbiq.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gficfhbqv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fanxiaobao.xyz/Article/details/gaigsxljj.sHtML

[T08] Kotlin：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/gnkuojhnm.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/goncgfevq.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fanxiaobao.xyz/Article/details/gsokyqsfm.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fanxiaobao.xyz/Article/details/ggwkzetvh.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gsezowiqw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gsmidtlwc.sHtML

[T11] Kotlin：协程
来源：http://blog.fanxiaobao.xyz/Article/details/gjvhcakzq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqvdimuit.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fanxiaobao.xyz/Article/details/gxlljwsii.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxbcrtffv.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fanxiaobao.xyz/Article/details/ggkuywlfp.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyaiblurs.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjackbmra.sHtML

for (i in 1..10) println(i)
来源：http://3g.fanxiaobao.xyz/Article/details/gvalqsclj.sHtML


<!-- 参考信息 -->