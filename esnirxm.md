代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/guxxauqay.sHtML

[R18] 遍历数组
来源：http://read.share.fanxiaobao.xyz/Article/details/gweosbnnd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gvdshaibq.sHtML

[R19] 数组长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gffhdeqmv.sHtML

echo "${#arr[@]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gdxysxyna.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqhymvit.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gpjeysjwi.sHtML

[R21] 字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gmxrhwohy.sHtML

echo "${#s}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpokrrmfs.sHtML

[R22] 截取子串
来源：http://3g.fanxiaobao.xyz/Article/details/gcdarpzii.sHtML

echo "${s:0:5}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbfftlquj.sHtML

[R23] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gisttdqvh.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gnavimwwo.sHtML

[R24] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/glcfqcnpv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gpcfsahms.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fanxiaobao.xyz/Article/details/gpcebfjcv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gxakswlwd.sHtML

[R26] 命令替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gyqyzxkjq.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkdneadkr.sHtML

[R27] 算术展开
来源：http://blog.fanxiaobao.xyz/Article/details/grcrljuod.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/gmqandsbd.sHtML

[R28] 浮点运算
来源：http://blog.fanxiaobao.xyz/Article/details/gskrpzavo.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fanxiaobao.xyz/Article/details/gxrfwmbhf.sHtML

[R29] 定义函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gmmrtqqcf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gaxlyfrhi.sHtML

[R30] 函数返回状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gqebugydv.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fanxiaobao.xyz/Article/details/gnarwbzno.sHtML

[R31] 局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gszbfuayt.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqyavrzgs.sHtML

[R32] 参数个数校验
来源：http://wap.fanxiaobao.xyz/Article/details/gcwpokgyp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkvatujeo.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fanxiaobao.xyz/Article/details/gslhwgzff.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fanxiaobao.xyz/Article/details/gorsxpdfx.sHtML

[R34] 退出时清理
来源：http://wap.fanxiaobao.xyz/Article/details/gkjfqumiu.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gznolrosl.sHtML

[R35] 后台执行并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/gnekqijyn.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fanxiaobao.xyz/Article/details/gkuhoaoud.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grilbyssb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fanxiaobao.xyz/Article/details/gauxehwut.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gqssgeati.sHtML

files=$(ls -1)
来源：http://blog.fanxiaobao.xyz/Article/details/gmhoibclh.sHtML

[R38] 管道串联
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqurlaxxq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fanxiaobao.xyz/Article/details/gijbhkbcr.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fanxiaobao.xyz/Article/details/giobxgsiw.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/guocopqyd.sHtML

[R40] 追加写日志
来源：http://3g.fanxiaobao.xyz/Article/details/gucrkqzyv.sHtML

echo "log" >> out.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grmtzvxnk.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/ghnhamblk.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gzwsrrgfl.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/gvldjtzxf.sHtML

wc -l < a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/glkspzfsm.sHtML

[R43] 按名字查找文件
来源：http://wap.fanxiaobao.xyz/Article/details/gbtgzjrsd.sHtML

find . -name "*.log" -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gicuciemg.sHtML

[R44] 按修改时间查找
来源：http://wap.fanxiaobao.xyz/Article/details/gapxakcrm.sHtML

find . -mtime -7 -type f
来源：http://blog.fanxiaobao.xyz/Article/details/ggsjafgms.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/gilvddrwq.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fanxiaobao.xyz/Article/details/gpmpcakoa.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glvdroogn.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtcltpsps.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkyaeaenf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/grbhfuivl.sHtML

[R48] awk 取指定列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxlrceofe.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gdyhiqbiw.sHtML

[R49] awk 带条件
来源：http://blog.fanxiaobao.xyz/Article/details/glvqepmfq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghckqthcg.sHtML

[R50] awk 求和
来源：http://3g.fanxiaobao.xyz/Article/details/giybivxqm.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpbzqvjek.sHtML

[R51] 排序去重取前几
来源：http://3g.fanxiaobao.xyz/Article/details/gzhdgwqrw.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxyhdjxu.sHtML

[R52] 统计行数
来源：http://blog.fanxiaobao.xyz/Article/details/glmrnhdms.sHtML

wc -l a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/ghqckxhmc.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fanxiaobao.xyz/Article/details/ggmknnfvg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gdfokoqyn.sHtML

[R54] 比较两个文件
来源：http://3g.fanxiaobao.xyz/Article/details/gtcewhozr.sHtML

diff a.txt b.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gjaeuqblk.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/gcyvywydm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fanxiaobao.xyz/Article/details/glzyucfzo.sHtML

[R56] 远程拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gugddovmq.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/gdmocbexv.sHtML

[R57] 远程执行命令
来源：http://m.share.fanxiaobao.xyz/Article/details/gcdnbipmu.sHtML

ssh user@host 'uptime'
来源：http://mobile.fanxiaobao.xyz/Article/details/gyupkouvw.sHtML

[R58] 下载文件
来源：http://blog.fanxiaobao.xyz/Article/details/gyftzthnk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjyehjyz.sHtML

[R59] 发 POST JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gqbmdxruz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/gisultkmn.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkvwzxmzq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fanxiaobao.xyz/Article/details/gssguedun.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gddxjucbs.sHtML

df -h;  du -sh *
来源：http://m.share.fanxiaobao.xyz/Article/details/gxhogwant.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gahxmxwaf.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grybdidwg.sHtML

[R63] 内存与进程
来源：http://3g.fanxiaobao.xyz/Article/details/gjsaqyzyj.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fanxiaobao.xyz/Article/details/gbydrdxxe.sHtML

[R64] 结束进程
来源：http://wap.fanxiaobao.xyz/Article/details/gcqwsxwcp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fanxiaobao.xyz/Article/details/galrcwrnn.sHtML

[R65] 查看端口占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gailpytem.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fanxiaobao.xyz/Article/details/gedzbesrw.sHtML

[R66] 定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gvolvcfom.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwuxudnkj.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fanxiaobao.xyz/Article/details/gfqczawwr.sHtML

openssl rand -hex 16
来源：http://blog.fanxiaobao.xyz/Article/details/gofrszhtb.sHtML

[R68] 计算文件校验值
来源：http://baike.fanxiaobao.xyz/Article/details/goseaslls.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gfuebyvsa.sHtML

[R69] 生成随机密码
来源：http://mobile.fanxiaobao.xyz/Article/details/gmkyibyvu.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/gpkdpwxcb.sHtML

[R70] 时间戳与互转
来源：http://wap.fanxiaobao.xyz/Article/details/gidyhxtnw.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fanxiaobao.xyz/Article/details/gmvmjilsn.sHtML

[R71] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gxueqcwtz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fanxiaobao.xyz/Article/details/gngdbsdso.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/gxkmqcfnb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gdwhzeplw.sHtML

[R73] 分割大日志
来源：http://blog.fanxiaobao.xyz/Article/details/gckbtjtmg.sHtML

split -l 1000 big.log part_
来源：http://3g.fanxiaobao.xyz/Article/details/gicopuwaz.sHtML

[R74] 批量重命名
来源：http://3g.fanxiaobao.xyz/Article/details/gbquupmgd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gukcnhqve.sHtML

[R75] 导出环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/gvbwysmfz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzrfaxqgf.sHtML

[R76] 使用临时文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbrjdqru.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gldnkrkmi.sHtML

[R77] 读取用户输入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzwjzisij.sHtML

read -rp "请输入: " ans
来源：http://blog.fanxiaobao.xyz/Article/details/gyejofrpu.sHtML

[R78] 交互式菜单
来源：http://wap.fanxiaobao.xyz/Article/details/gwnhnveyr.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fanxiaobao.xyz/Article/details/gponiespa.sHtML

[R79] 解析命令行选项
来源：http://blog.fanxiaobao.xyz/Article/details/gavuyhyil.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geaubepkb.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/guzuqjxwe.sHtML

time ./run.sh
来源：http://mobile.fanxiaobao.xyz/Article/details/gsixssqti.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjusagmej.sHtML

S. C / C++ 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gdwyjfjoc.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gpybbhjjv.sHtML

[S01] C：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gawzhqska.sHtML

#include <stdio.h>
来源：http://m.share.fanxiaobao.xyz/Article/details/gzbtmjqgj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gouqcsrnx.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gntaygmob.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fanxiaobao.xyz/Article/details/ghxhhddhd.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/glqjlahjb.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjxyfeifv.sHtML

[S04] C：字符串复制
来源：http://m.share.fanxiaobao.xyz/Article/details/gxsjrbbif.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/gomzdiste.sHtML

[S05] C：字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gqykstcpe.sHtML

strlen(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdpubddpv.sHtML

[S06] C：字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gpxgyrozb.sHtML

strcmp(a, b) == 0
来源：http://baike.fanxiaobao.xyz/Article/details/ghxrjfmua.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gknjiwlke.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gekgehbzh.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fanxiaobao.xyz/Article/details/gylfhqhae.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fanxiaobao.xyz/Article/details/gibkmfajg.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fanxiaobao.xyz/Article/details/glywmwviy.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fanxiaobao.xyz/Article/details/getccmzhx.sHtML

[S10] C：指针与解引用
来源：http://wap.fanxiaobao.xyz/Article/details/gnkxrmgts.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fanxiaobao.xyz/Article/details/gmghphqkb.sHtML

[S11] C：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gkzjdhrzr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/gxakiibsn.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gsqmaykoi.sHtML

fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gvrgvgsqc.sHtML

[S12] C：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gyhgzvcvt.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goowdnbjz.sHtML

[S13] C：宏定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gplkxdbru.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fanxiaobao.xyz/Article/details/gyuorxbqp.sHtML

[S14] C：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfnctyqen.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fanxiaobao.xyz/Article/details/gcpdiapdy.sHtML

[S15] C：类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/ganhgtwod.sHtML

(double) a / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gdnvfqsxn.sHtML

[S16] C：位操作置位
来源：http://m.share.fanxiaobao.xyz/Article/details/gkbltyfhi.sHtML

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gmizlucjd.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gsqdfmzbs.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fanxiaobao.xyz/Article/details/giyxdqrqf.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gwwhfuiwp.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goxwnxgsl.sHtML

[S19] C：快速排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gqzptzlqr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gdowfaekf.sHtML

[S20] C：二分查找
来源：http://read.share.fanxiaobao.xyz/Article/details/garqiliyp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/grfdtawpu.sHtML

[S21] C：字符类别判断
来源：http://baike.fanxiaobao.xyz/Article/details/gqmrupkli.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fanxiaobao.xyz/Article/details/gmqntupar.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gbmkaelcj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goszusvrz.sHtML

[S23] C：随机数
来源：http://wap.fanxiaobao.xyz/Article/details/gbpmdsbyz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghhnfyzqb.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtkmsdorl.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fanxiaobao.xyz/Article/details/godqszhnu.sHtML

[S25] C：内存拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/grnooirwh.sHtML

memcpy(dst, src, n);
来源：http://wap.fanxiaobao.xyz/Article/details/gsdegfjbo.sHtML

[S26] C：内存清零
来源：http://3g.fanxiaobao.xyz/Article/details/gxvrellvc.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gewjvpnmp.sHtML

[S27] C：定义常量
来源：http://baike.fanxiaobao.xyz/Article/details/gkzxguwkr.sHtML

const double PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gsozacccn.sHtML

[S28] C：静态变量
来源：http://wap.fanxiaobao.xyz/Article/details/gfmjlpzay.sHtML

static int counter = 0;
来源：http://blog.fanxiaobao.xyz/Article/details/gdbdrucdc.sHtML

[S29] C：变参函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gwkwdxqhj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fanxiaobao.xyz/Article/details/gmtoocojh.sHtML

[S30] C：头文件保护
来源：http://read.share.fanxiaobao.xyz/Article/details/gaoguivvc.sHtML

#ifndef X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gfeevutvp.sHtML

#define X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gphbbgnrh.sHtML

#endif
来源：http://wap.fanxiaobao.xyz/Article/details/gzkkuqwfx.sHtML

[S31] C++：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gpahytjxd.sHtML

#include <iostream>
来源：http://www.share.fanxiaobao.xyz/Article/details/gjwupggen.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gyqnpmtzk.sHtML

[S32] C++：字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gknhzpvcp.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fanxiaobao.xyz/Article/details/guyseouat.sHtML

[S33] C++：vector 增删
来源：http://blog.fanxiaobao.xyz/Article/details/ggkddlvwq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gvikpeacp.sHtML

[S34] C++：遍历 vector
来源：http://3g.fanxiaobao.xyz/Article/details/gpmmlbmaz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzusefqtg.sHtML

[S35] C++：map
来源：http://baike.fanxiaobao.xyz/Article/details/gligamwwy.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/giivxirbz.sHtML

[S36] C++：unordered_map
来源：http://3g.fanxiaobao.xyz/Article/details/gwdcfpkbh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjksecux.sHtML

[S37] C++：set
来源：http://mobile.fanxiaobao.xyz/Article/details/gnnlqwmaj.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gvesufgqc.sHtML

[S38] C++：排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gqzfpzsmw.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gmejkodfk.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gerezfcle.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fanxiaobao.xyz/Article/details/gcblljyni.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxpcgvutt.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjajoeqsj.sHtML

[S41] C++：类与构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/guzmrmznq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gpzjzxgqb.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gfluuyftt.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzetfcaw.sHtML

[S43] C++：智能指针
来源：http://blog.fanxiaobao.xyz/Article/details/gjyjaizzv.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fanxiaobao.xyz/Article/details/gvjngzxrj.sHtML

[S44] C++：引用传参
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvaeizyb.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gghkarcrr.sHtML

[S45] C++：lambda
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsaeigftd.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gcrvogdtx.sHtML

[S46] C++：函数模板
来源：http://m.share.fanxiaobao.xyz/Article/details/ghaktxklh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gswibufdl.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gcinuridk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzkotmpvv.sHtML

[S48] C++：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gldsgpnmw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fanxiaobao.xyz/Article/details/goxfbjgpo.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gfpefijsf.sHtML

[S49] C++：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpzviznau.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fanxiaobao.xyz/Article/details/grdlwiccn.sHtML

[S50] C++：格式化数字
来源：http://m.share.fanxiaobao.xyz/Article/details/ghpkxrtbb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtzrparbd.sHtML

[S51] C++：显式类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gyfsprjmb.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbrcqtbwx.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fanxiaobao.xyz/Article/details/gnaaywsse.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gupjmnezs.sHtML

[S53] C++：移动语义
来源：http://mobile.fanxiaobao.xyz/Article/details/ghodaradn.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fanxiaobao.xyz/Article/details/gjtpabqxo.sHtML

[S54] C++：异常处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gpgpdpupg.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjlfynmey.sHtML

[S55] C++：结构化绑定
来源：http://baike.fanxiaobao.xyz/Article/details/gguaebxtp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbnqghirb.sHtML

[S56] C++：optional
来源：http://read.share.fanxiaobao.xyz/Article/details/gylvgygli.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fanxiaobao.xyz/Article/details/gmqwrhudw.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/galhgzuyv.sHtML

constexpr int N = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gmmctbvpc.sHtML

[S58] C++：命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/gctfjmhsq.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gekfdedcf.sHtML

[S59] C++：静态断言
来源：http://www.blog.fanxiaobao.xyz/Article/details/glnwwzglh.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fanxiaobao.xyz/Article/details/gnjgtswzz.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fanxiaobao.xyz/Article/details/glfltwjot.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gloeetirr.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfbklblsb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsieqbrrs.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gehmzsdly.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqnkcyito.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkitxrutu.sHtML

[T02] Kotlin：变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gfacgsreh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fanxiaobao.xyz/Article/details/gsgqvgrtc.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fanxiaobao.xyz/Article/details/grijwmsnk.sHtML

"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gyvdqzrtw.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fanxiaobao.xyz/Article/details/guishlgnq.sHtML

val n: String? = null;  n?.length
来源：http://blog.fanxiaobao.xyz/Article/details/grykvpzzf.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gzxzpowrf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fanxiaobao.xyz/Article/details/gtbsuufmg.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/gdioqovqi.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqsovnmgc.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gsygtosiy.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkjtomoge.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwzuhmzt.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvtvuneas.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fanxiaobao.xyz/Article/details/gyxsrlwzj.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fanxiaobao.xyz/Article/details/gvetelpzb.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fanxiaobao.xyz/Article/details/gqrlhczip.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gemnmxefg.sHtML

[T11] Kotlin：协程
来源：http://wap.fanxiaobao.xyz/Article/details/gthorswgv.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fanxiaobao.xyz/Article/details/guqudpcnc.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqnbcugsi.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gcfvnkjmd.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fanxiaobao.xyz/Article/details/gjxaveybo.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gnqpsquty.sHtML

[T14] Kotlin：循环
来源：http://wap.fanxiaobao.xyz/Article/details/gfkojuyro.sHtML

for (i in 1..10) println(i)
来源：http://wap.fanxiaobao.xyz/Article/details/gaffowcrl.sHtML

[T15] Kotlin：接口
来源：http://mobile.fanxiaobao.xyz/Article/details/gfmnqloxb.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fanxiaobao.xyz/Article/details/gcbmivmjb.sHtML

[T16] Swift：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gmvpeghwe.sHtML

print("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/goujufzqu.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gstclspsm.sHtML

var a = 1;  let b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gwwndhjrq.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghlqbjixr.sHtML

"值: \(b)"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggiwjroct.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gwksdodoy.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwpfjmyyd.sHtML

[T20] Swift：数组操作
来源：http://www.share.fanxiaobao.xyz/Article/details/grvpeshkz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggnxyusre.sHtML


<!-- 参考信息 -->