代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gshutvffl.sHtML

[R14] C 风格 for
来源：http://mobile.fanxiaobao.xyz/Article/details/gsixqurme.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/glhsvvede.sHtML

[R15] while 逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gcpnvnubx.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gyzqmqjfl.sHtML

[R16] until 等待条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqhoulbl.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gxaobvtvm.sHtML

[R17] 数组定义与取值
来源：http://blog.fanxiaobao.xyz/Article/details/goohxpdug.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gegopwrny.sHtML

[R18] 遍历数组
来源：http://wap.fanxiaobao.xyz/Article/details/gzstqacax.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gkrnkcjfu.sHtML

[R19] 数组长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbdcrhfiu.sHtML

echo "${#arr[@]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gkwkccoiz.sHtML

[R20] 关联数组（字典）
来源：http://wap.fanxiaobao.xyz/Article/details/glurbrxgs.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gilhpznws.sHtML

[R21] 字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gomyvoogf.sHtML

echo "${#s}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gykragqxd.sHtML

[R22] 截取子串
来源：http://baike.fanxiaobao.xyz/Article/details/gxabsjqmx.sHtML

echo "${s:0:5}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gxvfscsyb.sHtML

[R23] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjwwedoyl.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzgavcvte.sHtML

[R24] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gsxtuuehg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/gyhackqav.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fanxiaobao.xyz/Article/details/grxlnpzqb.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fanxiaobao.xyz/Article/details/gshulnmbs.sHtML

[R26] 命令替换
来源：http://wap.fanxiaobao.xyz/Article/details/gcfedywxw.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fanxiaobao.xyz/Article/details/ggywluvlp.sHtML

[R27] 算术展开
来源：http://wap.fanxiaobao.xyz/Article/details/gmvuawsew.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/ghyinnfpq.sHtML

[R28] 浮点运算
来源：http://blog.fanxiaobao.xyz/Article/details/gfswjaklq.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fanxiaobao.xyz/Article/details/gjwqntkip.sHtML

[R29] 定义函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gjrhibhxc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fanxiaobao.xyz/Article/details/guvcrnbsh.sHtML

[R30] 函数返回状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/grnbfnbuk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fanxiaobao.xyz/Article/details/gsypapkzd.sHtML

[R31] 局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkeitaffp.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gmzcfyevz.sHtML

[R32] 参数个数校验
来源：http://m.share.fanxiaobao.xyz/Article/details/gmyvslxax.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxvuvmdy.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fanxiaobao.xyz/Article/details/gydbhnckw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fanxiaobao.xyz/Article/details/gqemgasrn.sHtML

[R34] 退出时清理
来源：http://blog.fanxiaobao.xyz/Article/details/glbzwkpja.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gdykbsirx.sHtML

[R35] 后台执行并等待
来源：http://3g.fanxiaobao.xyz/Article/details/gxbsdwdks.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gplwwmuht.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnzpohaur.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbwfzymgp.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gfcqlohdt.sHtML

files=$(ls -1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwialvgou.sHtML

[R38] 管道串联
来源：http://blog.fanxiaobao.xyz/Article/details/grlkltcga.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fanxiaobao.xyz/Article/details/glczwvdqd.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fanxiaobao.xyz/Article/details/grgydxaaw.sHtML

cmd > out.log 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gwxhxnkkk.sHtML

[R40] 追加写日志
来源：http://blog.fanxiaobao.xyz/Article/details/gqerfverx.sHtML

echo "log" >> out.log
来源：http://3g.fanxiaobao.xyz/Article/details/gvtnsrwue.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gibirmekg.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gfrdtzmsk.sHtML

[R42] 输入重定向
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwcctwpw.sHtML

wc -l < a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gaokvvbqm.sHtML

[R43] 按名字查找文件
来源：http://wap.fanxiaobao.xyz/Article/details/gikxxhzlq.sHtML

find . -name "*.log" -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gehzbhhyn.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzrmutacd.sHtML

find . -mtime -7 -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/ghnygrrdp.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gehmwfedn.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fanxiaobao.xyz/Article/details/ggsoqkkgk.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/gzsemocrr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fanxiaobao.xyz/Article/details/gzdjtfsho.sHtML

[R47] sed 单行替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gzbvdkpes.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpbbjlmxu.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjgqzyom.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvwhgdqew.sHtML

[R49] awk 带条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gugzpdxqn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fanxiaobao.xyz/Article/details/glyecuock.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqmewtfnl.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/grdotemqx.sHtML

[R51] 排序去重取前几
来源：http://mobile.fanxiaobao.xyz/Article/details/gavcwsrbn.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fanxiaobao.xyz/Article/details/gstdyfwzr.sHtML

[R52] 统计行数
来源：http://wap.fanxiaobao.xyz/Article/details/gmvlspdny.sHtML

wc -l a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gackhvsdh.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fanxiaobao.xyz/Article/details/gxufjfgyc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbkjpshro.sHtML

[R54] 比较两个文件
来源：http://3g.fanxiaobao.xyz/Article/details/goqczckrv.sHtML

diff a.txt b.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzcqxjjll.sHtML

[R55] 压缩与解压
来源：http://mobile.fanxiaobao.xyz/Article/details/gcvgebexr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fanxiaobao.xyz/Article/details/gndxutdkh.sHtML

[R56] 远程拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gwzkdernw.sHtML

scp file user@host:/path/
来源：http://blog.fanxiaobao.xyz/Article/details/gttfksvsa.sHtML

[R57] 远程执行命令
来源：http://blog.fanxiaobao.xyz/Article/details/ghkqavqly.sHtML

ssh user@host 'uptime'
来源：http://read.share.fanxiaobao.xyz/Article/details/giumswifw.sHtML

[R58] 下载文件
来源：http://wap.fanxiaobao.xyz/Article/details/gfwipldxl.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/gzsjzmeua.sHtML

[R59] 发 POST JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/guutkkdnc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gusxjguup.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gdfscpths.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gghunaoxr.sHtML

[R61] 磁盘占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvoqvdmd.sHtML

df -h;  du -sh *
来源：http://blog.fanxiaobao.xyz/Article/details/gpbktuxag.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmeijozb.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fanxiaobao.xyz/Article/details/grwpsgign.sHtML

[R63] 内存与进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gnauehxbn.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fanxiaobao.xyz/Article/details/gtfzfxixq.sHtML

[R64] 结束进程
来源：http://www.share.fanxiaobao.xyz/Article/details/glybmtjng.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fanxiaobao.xyz/Article/details/gfjrinwtq.sHtML

[R65] 查看端口占用
来源：http://3g.fanxiaobao.xyz/Article/details/gwgfmhlky.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fanxiaobao.xyz/Article/details/gdtsfjkim.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gaopgmioo.sHtML

crontab -e;  crontab -l
来源：http://wap.fanxiaobao.xyz/Article/details/gbccrhelt.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmpofogjh.sHtML

openssl rand -hex 16
来源：http://mobile.fanxiaobao.xyz/Article/details/gaplxtajs.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gugzhjzyz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpdahxiut.sHtML

[R69] 生成随机密码
来源：http://mobile.fanxiaobao.xyz/Article/details/gevgtpahn.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fanxiaobao.xyz/Article/details/gaaibkbcs.sHtML

[R70] 时间戳与互转
来源：http://blog.fanxiaobao.xyz/Article/details/gawmfmixx.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fanxiaobao.xyz/Article/details/gcagfxrft.sHtML

[R71] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggczeldea.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijqadndc.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/gbdnpojtt.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gumyhxzup.sHtML

[R73] 分割大日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gjosszqqc.sHtML

split -l 1000 big.log part_
来源：http://www.share.fanxiaobao.xyz/Article/details/gaftugteb.sHtML

[R74] 批量重命名
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwpwpkno.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gcpsgsvwh.sHtML

[R75] 导出环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/ggtsaeyvr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fanxiaobao.xyz/Article/details/gpvkdkmjm.sHtML

[R76] 使用临时文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gruqjspmr.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gkeanscks.sHtML

[R77] 读取用户输入
来源：http://blog.fanxiaobao.xyz/Article/details/gyrymfokl.sHtML

read -rp "请输入: " ans
来源：http://mobile.fanxiaobao.xyz/Article/details/gqpczzdtg.sHtML

[R78] 交互式菜单
来源：http://blog.fanxiaobao.xyz/Article/details/gufwqhjcd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fanxiaobao.xyz/Article/details/gdcbcesth.sHtML

[R79] 解析命令行选项
来源：http://read.share.fanxiaobao.xyz/Article/details/gkqbjyqgy.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fanxiaobao.xyz/Article/details/gqfqtubyf.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fanxiaobao.xyz/Article/details/ganpktoey.sHtML

time ./run.sh
来源：http://wap.fanxiaobao.xyz/Article/details/gcurcqwmx.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gisdaobaj.sHtML

S. C / C++ 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gykpfqjqi.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gxbyiipdb.sHtML

[S01] C：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/giisdoqdh.sHtML

#include <stdio.h>
来源：http://wap.fanxiaobao.xyz/Article/details/gngsheyaz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fanxiaobao.xyz/Article/details/ghsytolgu.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnnpejmuc.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyieohabk.sHtML

[S03] C：读入整数
来源：http://baike.fanxiaobao.xyz/Article/details/gdmxuiltj.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtrdnvait.sHtML

[S04] C：字符串复制
来源：http://wap.fanxiaobao.xyz/Article/details/gqtsfsvwi.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fanxiaobao.xyz/Article/details/gagesuawi.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gmutnhrqs.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/ghihuwhuc.sHtML

[S06] C：字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gojbtfajk.sHtML

strcmp(a, b) == 0
来源：http://m.share.fanxiaobao.xyz/Article/details/gmcwbjlmx.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gntxwpmve.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fanxiaobao.xyz/Article/details/gzflfegab.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggeahabfz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fanxiaobao.xyz/Article/details/gbyhwtjbs.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fanxiaobao.xyz/Article/details/gcgkceedm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fanxiaobao.xyz/Article/details/gkxdkxiyu.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gikogiilz.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fanxiaobao.xyz/Article/details/gcivrtqtg.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggwzfeabj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fanxiaobao.xyz/Article/details/gdgmuhutj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghwrxbapj.sHtML

fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/glwnotzup.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gkmopqtjt.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gqnpxyohh.sHtML

[S13] C：宏定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gprdehwhx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fanxiaobao.xyz/Article/details/gzbycwxiw.sHtML

[S14] C：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gnwxcpcoq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fanxiaobao.xyz/Article/details/gmfmpkuyb.sHtML

[S15] C：类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gzgtybfvx.sHtML

(double) a / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gmwdglcaz.sHtML

[S16] C：位操作置位
来源：http://www.share.fanxiaobao.xyz/Article/details/gixviuqtt.sHtML

x |= (1 << 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdsbyzygp.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gxheoqvnz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fanxiaobao.xyz/Article/details/gvwfpabzx.sHtML

[S18] C：命令行参数
来源：http://3g.fanxiaobao.xyz/Article/details/gjvgrrqek.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzjeotkxm.sHtML

[S19] C：快速排序
来源：http://wap.fanxiaobao.xyz/Article/details/gwlusoprm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxjgamrlo.sHtML

[S20] C：二分查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbtebura.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gedqaqmrf.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/ghefrnmqn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fanxiaobao.xyz/Article/details/gbkthmpce.sHtML

[S22] C：字符串转数字
来源：http://baike.fanxiaobao.xyz/Article/details/gpkvpanwe.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwofkrrwd.sHtML

[S23] C：随机数
来源：http://read.share.fanxiaobao.xyz/Article/details/gwiirfmfw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fanxiaobao.xyz/Article/details/grcdfyrnb.sHtML

[S24] C：获取本地时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gvgowddvf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fanxiaobao.xyz/Article/details/gdsuiczvd.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/geiuxlfgt.sHtML

memcpy(dst, src, n);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbxgliudi.sHtML

[S26] C：内存清零
来源：http://3g.fanxiaobao.xyz/Article/details/gluxyyuic.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbhwbqayt.sHtML

[S27] C：定义常量
来源：http://wap.fanxiaobao.xyz/Article/details/gjjxvjbqz.sHtML

const double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwwhgwtgz.sHtML

[S28] C：静态变量
来源：http://wap.fanxiaobao.xyz/Article/details/gryieuyzo.sHtML

static int counter = 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/glasnvzns.sHtML

[S29] C：变参函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaaytqphm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjevhnjin.sHtML

[S30] C：头文件保护
来源：http://baike.fanxiaobao.xyz/Article/details/gxirwhuoj.sHtML

#ifndef X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdimtoers.sHtML

#define X_H
来源：http://blog.fanxiaobao.xyz/Article/details/glzoksacz.sHtML

#endif
来源：http://blog.fanxiaobao.xyz/Article/details/gnedvunlb.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhiekfwr.sHtML

#include <iostream>
来源：http://wap.fanxiaobao.xyz/Article/details/gtogtvmjr.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gerbcxtpa.sHtML

[S32] C++：字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gxqncpobt.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fanxiaobao.xyz/Article/details/gzjbvxrmn.sHtML

[S33] C++：vector 增删
来源：http://mobile.fanxiaobao.xyz/Article/details/gujoaoels.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzujffcqg.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gseejscmq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbcjazyko.sHtML

[S35] C++：map
来源：http://www.share.fanxiaobao.xyz/Article/details/gdtaitkxn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggutzkbbt.sHtML

[S36] C++：unordered_map
来源：http://baike.fanxiaobao.xyz/Article/details/gtlentomx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gxsqqfxcm.sHtML

[S37] C++：set
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnpeudnuw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gxfusapln.sHtML

[S38] C++：排序
来源：http://baike.fanxiaobao.xyz/Article/details/gvudsvuzg.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/goacalmuo.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxeyysnj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gouedpbsb.sHtML

[S40] C++：查找元素
来源：http://wap.fanxiaobao.xyz/Article/details/gbqnkpbyo.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gcxetbaqg.sHtML

[S41] C++：类与构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/ggxarqqci.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gmehzknpv.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fanxiaobao.xyz/Article/details/gjvtklegc.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fanxiaobao.xyz/Article/details/gkwfjkosk.sHtML

[S43] C++：智能指针
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcetbkayy.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdfnzgyom.sHtML

[S44] C++：引用传参
来源：http://read.share.fanxiaobao.xyz/Article/details/gawgpmjel.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdstxncjo.sHtML

[S45] C++：lambda
来源：http://blog.fanxiaobao.xyz/Article/details/ggcwzbrjr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fanxiaobao.xyz/Article/details/gyaffnwhs.sHtML

[S46] C++：函数模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gccodewur.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzlyttjhd.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/glbflunyf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxyqzgdps.sHtML

[S48] C++：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gugqfmkry.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnfbuvqed.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnejnlkuh.sHtML

[S49] C++：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gtwxjqvad.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/guktumdlm.sHtML

[S50] C++：格式化数字
来源：http://www.share.fanxiaobao.xyz/Article/details/ggpltkiad.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gyqlwwtfp.sHtML

[S51] C++：显式类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gebywqdct.sHtML

static_cast<double>(a) / b
来源：http://blog.fanxiaobao.xyz/Article/details/gkilaxsnt.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fanxiaobao.xyz/Article/details/gglohbota.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gisvyjgzu.sHtML

[S53] C++：移动语义
来源：http://blog.fanxiaobao.xyz/Article/details/gepjeivea.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvgttzont.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gysgddbow.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gylrpykbz.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gnwphqmag.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gtygmzysr.sHtML

[S56] C++：optional
来源：http://blog.fanxiaobao.xyz/Article/details/gxknjxwcb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gclajgsgs.sHtML

[S57] C++：编译期常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxmgqacg.sHtML

constexpr int N = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gsewvtkse.sHtML

[S58] C++：命名空间
来源：http://baike.fanxiaobao.xyz/Article/details/gmuueqdks.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnuesgrtf.sHtML

[S59] C++：静态断言
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzxqalsxu.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fanxiaobao.xyz/Article/details/gocpohjnd.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqcioeebb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/giqlruvee.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gdaehfdbb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fanxiaobao.xyz/Article/details/gyrvwvfss.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gwonvztra.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gvtzfotcf.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpgutiuib.sHtML

[T02] Kotlin：变量
来源：http://blog.fanxiaobao.xyz/Article/details/gkpvvinzf.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gauypsbqi.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gkbdtouuz.sHtML

"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gxcxgztel.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fanxiaobao.xyz/Article/details/gpecgxjxs.sHtML

val n: String? = null;  n?.length
来源：http://wap.fanxiaobao.xyz/Article/details/gmbuvxmnk.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkvcscqed.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fanxiaobao.xyz/Article/details/gjfurtbxu.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/gjylihwoj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gikedyidz.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gksvkmyvi.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fanxiaobao.xyz/Article/details/gwliaitof.sHtML

[T08] Kotlin：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/gboeqbpai.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkzoehttl.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gexsiqmng.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fanxiaobao.xyz/Article/details/gqarbqhvm.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gsnmffale.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fanxiaobao.xyz/Article/details/gsjekvhby.sHtML

[T11] Kotlin：协程
来源：http://read.share.fanxiaobao.xyz/Article/details/gbqzigafd.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fanxiaobao.xyz/Article/details/gpxlagoxz.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fanxiaobao.xyz/Article/details/gfctoonmo.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gtbynxtln.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fanxiaobao.xyz/Article/details/gujspmcer.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gucdepsph.sHtML

[T14] Kotlin：循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gboyvtldx.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/guodeqqvu.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gotxeultq.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fanxiaobao.xyz/Article/details/gpjdrqxch.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcjywfpuz.sHtML

print("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gqtvxafwg.sHtML


<!-- 参考信息 -->