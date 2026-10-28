代发 wailian999

set -euo pipefail
来源：http://hz.ywan-chungtsiang.top/gtmhxaiywr.html

[R02] 变量赋值与使用
来源：http://hz.yj20258888.top/gtvmvgrrhd.html

name="Tom"; echo "$name"
来源：http://hz.bjfxy.top/gttkpdiwnd.html

[R03] 只读变量
来源：http://hz.hysaishi.cn/gtxywpqlar.html

readonly PI=3.14
来源：http://hz.dianchejie.cn/gttxdmdbtt.html

[R04] 位置参数
来源：http://hz.jqgufenzy.top/gtjzcfzmub.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.nanxuanxn.top/gtchebqrtc.html

[R05] 参数默认值
来源：http://hz.jinghuilouyu.cn/gtzcqwuaip.html

name="${1:-default}"
来源：http://hz.yonumen.top/gtukuvkkql.html

[R06] 判断命令是否存在
来源：http://hz.shanyushiyangtech.top/gtjpimkcaj.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.52xcode.cn/gtxxmunuby.html

[R07] if 判断文件
来源：http://hz.pengpengdd.cyou/gtcmxhbdqz.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.chenjidiqi.icu/gtsliorwlq.html

[R08] 数值比较
来源：http://hz.xuanzx.com/gtxjqgvhnd.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.zhijiandao.cn/gtqrelkbnp.html

[R09] 字符串比较
来源：http://hz.nanxinkj.top/gteixagpop.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.kuanghao11.cn/gthyibavee.html

[R10] 正则匹配
来源：http://hz.zhaomingkeji.xyz/gtgnnvpipg.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.gzhubu.top/gtuteeukqv.html

[R11] case 多分支
来源：http://hz.xinyue.icu/gtyruflhln.html

case "$1" in
来源：http://hz.wangdashe.top/gtzzabgedl.html

start) echo "启动" ;;
来源：http://hz.zhaomingkeji.xyz/gtqnxbrfpa.html

stop)  echo "停止" ;;
来源：http://hz.yj20258888.top/gtpoizimdo.html

*)     echo "未知命令" ;;
来源：http://hz.bjfxy.top/gtbmtygkkf.html

esac
来源：http://hz.yanxiufei.cn/gtftktzgwz.html

[R12] for 遍历文件
来源：http://hz.xuetiantiany.cn/gtymnlqjzp.html

for f in *.txt; do echo "$f"; done
来源：http://hz.316326.xyz/gtovlzplal.html

[R13] for 计数循环
来源：http://hz.snrcjt.cn/gtkecuvpnv.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.yangfankeji.com/gtgasdbhwq.html

[R14] C 风格 for
来源：http://hz.ybcxt.top/gtnzifbqqk.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.cucudq.cn/gtakozksau.html

[R15] while 逐行读文件
来源：http://hz.ywan-chungtsiang.top/gtmifjydmd.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.redwolf501.top/gtujwnrbap.html

[R16] until 等待条件
来源：http://hz.daxiang520.top/gtqgzomlpb.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.dianchejie.cn/gtvdpkhjof.html

[R17] 数组定义与取值
来源：http://hz.zhijiandao.cn/gtudiartws.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.xziqi.cn/gtcmiitrfy.html

[R18] 遍历数组
来源：http://hz.tanke756.top/gthwlwkiof.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.gotoacloud.top/gthrfmrzrq.html

[R19] 数组长度
来源：http://hz.havefunace.top/gtgigkchgv.html

echo "${#arr[@]}"
来源：http://hz.jqgufenzy.top/gtffbbrvhj.html

[R20] 关联数组（字典）
来源：http://hz.0kj1m.cn/gtlibsvohq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.hongshengwenyu.top/gtaldpozkf.html

[R21] 字符串长度
来源：http://hz.yanxiufei.cn/gtqqzgzmxh.html

echo "${#s}"
来源：http://hz.chenzaomai.com/gtxmstpixb.html

[R22] 截取子串
来源：http://hz.shanyushiyangkeji.top/gtykiduwdt.html

echo "${s:0:5}"
来源：http://hz.chenjidiqi.icu/gtulvxaycf.html

[R23] 字符串替换
来源：http://hz.svipenyu.cn/gtaqigedyp.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.gaohongyu789.top/gtlzxzdnwk.html

[R24] 大小写转换
来源：http://hz.smart0.xyz/gtktwwcbhx.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.hfpthk.cn/gtvzwxhioc.html

[R25] 去后缀 / 去前缀
来源：http://hz.hfpthk.cn/gtlxtfzddl.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.xylfe.cn/gtwwxgaatv.html

[R26] 命令替换
来源：http://hz.jianghu66.top/gtmjmqkopx.html

now=$(date +%F); echo "$now"
来源：http://hz.tianlin.xyz/gtqsufritx.html

[R27] 算术展开
来源：http://hz.svipenyu.cn/gthevzlygl.html

echo $((1 + 2 * 3))
来源：http://hz.kuanghao11.cn/gtkvcattwv.html

[R28] 浮点运算
来源：http://hz.aibaodan.cn/gtgwdzwjir.html

echo "scale=2; 10/3" | bc
来源：http://hz.guowangkeji.top/gtpeqejbwe.html

[R29] 定义函数
来源：http://hz.wangshuangyany.cn/gtumutgyha.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.shangyingyoupin.top/gtsqljrmzh.html

[R30] 函数返回状态码
来源：http://hz.hfpthk.cn/gtmzxgcaks.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.zhongyouzk.top/gtoqsqpykk.html

[R31] 局部变量
来源：http://hz.pengpengdd.cyou/gtuefpcbod.html

f() { local x=1; echo "$x"; }
来源：http://hz.aibaodan.cn/gttjchulsr.html

[R32] 参数个数校验
来源：http://hz.fengsongda.top/gtobtpkhba.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.hongshengwenyu.top/gtdiivkvpg.html

[R33] 捕获错误并提示行号
来源：http://hz.shuidangran.top/gticxfeibs.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.dianchejie.cn/gtrqcbkqku.html

[R34] 退出时清理
来源：http://hz.yuxming.cn/gtsxtplqnh.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.jqgfzy.top/gtyyiorlrh.html

[R35] 后台执行并等待
来源：http://hz.ywan-chungtsiang.top/gtgbwbfkqy.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.yuxming.cn/gtjgeupofa.html

[R36] 并发执行多个任务
来源：http://hz.xylfe.cn/gtenzyzvcj.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.tanke756.top/gtoaplwcnq.html

[R37] 把输出赋给变量
来源：http://hz.kuanghao11.cn/gtgndvetui.html

files=$(ls -1)
来源：http://hz.c1oappe.top/gtbqjvdaiw.html

[R38] 管道串联
来源：http://hz.hnqzz.top/gtkvnqdkmm.html

cat a.txt | grep -i error | wc -l
来源：http://hz.hywenlv.cn/gtttkufvea.html

[R39] 重定向标准输出与错误
来源：http://hz.iojbl.cn/gtvjbzdkdh.html

cmd > out.log 2>&1
来源：http://hz.aizwys.cn/gthiygosoo.html

[R40] 追加写日志
来源：http://hz.xylfe.cn/gtzrslddnt.html

echo "log" >> out.log
来源：http://hz.mhx1999.top/gtisectxei.html

[R41] 丢弃输出
来源：http://hz.fzhhl.top/gtfanlnzvr.html

cmd >/dev/null 2>&1
来源：http://hz.guannengcc.top/gtzvzqzqcw.html

[R42] 输入重定向
来源：http://hz.gotoacloud.top/gtvkwdnest.html

wc -l < a.txt
来源：http://hz.jinyuanbaomall.cn/gtnrtgnjfc.html

[R43] 按名字查找文件
来源：http://hz.snrcjt.cn/gtaiqmyjfg.html

find . -name "*.log" -type f
来源：http://hz.aizwys.cn/gtzmsgqkcv.html

[R44] 按修改时间查找
来源：http://hz.fengsongda.top/gtwffknudw.html

find . -mtime -7 -type f
来源：http://hz.quarkkingdee.top/gtdvpjrkfe.html

[R45] 批量删除
来源：http://hz.shanyushiyangtech.top/gtgywabjhd.html

find . -name "*.tmp" -delete
来源：http://hz.nanxinkj.top/gtbgqhwnfl.html

[R46] 递归替换文件内容
来源：http://hz.jqgufenzy.top/gtgmenmpnl.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.sysykeji.top/gtkfzbqfzq.html

[R47] sed 单行替换
来源：http://hz.jinyuanbaomall.cn/gtmctbhwex.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.xuetiantiany.cn/gtunqyochl.html

[R48] awk 取指定列
来源：http://hz.xziqi.cn/gtbeygtqsq.html

awk '{print $1, $3}' a.txt
来源：http://hz.yueranfly.top/gthvpjbtyy.html

[R49] awk 带条件
来源：http://hz.jqgufenzy.top/gtjilnprbl.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.jqgfzy.top/gtzekohmpm.html

[R50] awk 求和
来源：http://hz.yonumen.top/gthjwwwdhy.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.wangshuangyany.cn/gtehyeickj.html

[R51] 排序去重取前几
来源：http://hz.xinyue.icu/gtvydbakmk.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.jlsjyb.cn/gtloscwmwk.html

[R52] 统计行数
来源：http://hz.zdqjudy.top/gtgpanouyy.html

wc -l a.txt
来源：http://hz.chenlongwang.top/gtenvqxylq.html

[R53] 查看文件头与实时尾
来源：http://hz.kuanghao11.cn/gtoaqcseyn.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.jyoumei.cn/gtokhxevtq.html

[R54] 比较两个文件
来源：http://hz.zhiwuduotai.top/gtdkretuxz.html

diff a.txt b.txt
来源：http://hz.hammf.cn/gtyiymqqau.html

[R55] 压缩与解压
来源：http://hz.shuidangran.top/gtrtxuzqyo.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.nanxinkj.top/gtchdnfyzr.html

[R56] 远程拷贝
来源：http://hz.snrcjt.cn/gtgmaemlag.html

scp file user@host:/path/
来源：http://hz.zhongyouzk.top/gtpsjzffma.html

[R57] 远程执行命令
来源：http://hz.daxiang520.top/gttnsudkro.html

ssh user@host 'uptime'
来源：http://hz.yangfankeji.com/gthdqyemmf.html

[R58] 下载文件
来源：http://hz.jinqigfzy.top/gtyvzrxwhn.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.guannengcc.top/gtpbwpxnch.html

[R59] 发 POST JSON
来源：http://hz.tianlin.xyz/gtzwcsdkjn.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.9152youxi.cn/gtugdzknbp.html

[R60] 只看 HTTP 状态码
来源：http://hz.9152youxi.cn/gtzvvixbph.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.yvedp.cn/gtcaqstkce.html

[R61] 磁盘占用
来源：http://hz.yj202588.top/gtqpedwdvl.html

df -h;  du -sh *
来源：http://hz.sufxvd.cn/gtovjqxrjd.html

[R62] 找最占空间的文件
来源：http://hz.mhx1999.top/gtzuqxpzmv.html

du -ah . | sort -rh | head -10
来源：http://hz.cdnleiting.top/gtunfuybfp.html

[R63] 内存与进程
来源：http://hz.mhx1999.top/gtnooqtkwz.html

free -h;  ps aux | grep nginx
来源：http://hz.yongpay.top/gtvcnvudpm.html

[R64] 结束进程
来源：http://hz.shanyushiyangkeji.top/gtrkciezkk.html

kill -9 $(pgrep -f app.py)
来源：http://hz.redwolf501.top/gtwvsfhvhy.html

[R65] 查看端口占用
来源：http://hz.zhaomingkeji.xyz/gtbhxvixnk.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.ehwqpu.com/gtunmicdwm.html

[R66] 定时任务
来源：http://hz.52xcode.cn/gtxdylugby.html

crontab -e;  crontab -l
来源：http://hz.ydjk.org.cn/gtxevtzdko.html

[R67] 生成随机十六进制串
来源：http://hz.cheryme.top/gtvkfizzfr.html

openssl rand -hex 16
来源：http://hz.nanxuanxn.top/gtzkkuukip.html

[R68] 计算文件校验值
来源：http://hz.yangfankeji.com/gthfygsegp.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.zhongyouzk.top/gtrozmbeia.html

[R69] 生成随机密码
来源：http://hz.ehwqpu.com/gtienhdbzm.html

head -c 16 /dev/urandom | base64
来源：http://hz.yuanzhike.top/gtcahhefea.html

[R70] 时间戳与互转
来源：http://hz.yueranfly.top/gthyfsnbcq.html

date +%s;  date -d @1700000000
来源：http://hz.zhijiandao.cn/gtjjtuxxwc.html

[R71] 日期格式化
来源：http://hz.vqdsnc.cn/gtooimhanq.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.mhx1999.top/gtiabjqlfs.html

[R72] 等待端口就绪
来源：http://hz.nwbrower.top/gtazkwqowc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.jlsjyb.cn/gtbhnyhjxj.html

[R73] 分割大日志
来源：http://hz.jinyuanbaomall.cn/gtnnwyzbnw.html

split -l 1000 big.log part_
来源：http://hz.hysaishi.cn/gtraioulqv.html

[R74] 批量重命名
来源：http://hz.quarkkingdee.top/gtfnacyznl.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.9152youxi.cn/gtcrfasule.html

[R75] 导出环境变量
来源：http://hz.birdmap.top/gtnmpjffwr.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.chenlongwang.top/gtrqhouwdr.html

[R76] 使用临时文件
来源：http://hz.gaohongyu789.top/gtfrzgsrtv.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.tian-w.cn/gtnjlorgav.html

[R77] 读取用户输入
来源：http://hz.tian-w.cn/gtvdutnfvl.html

read -rp "请输入: " ans
来源：http://hz.ehwqpu.com/gtabrbqzry.html

[R78] 交互式菜单
来源：http://hz.hysaishi.cn/gttqepzgcb.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.sweek.top/gtkxdkdtfw.html

[R79] 解析命令行选项
来源：http://hz.zhaomingkeji.xyz/gtsvmvqwps.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.jinyuanbaomall.cn/gtxdvnzcvc.html

[R80] 查看脚本执行耗时
来源：http://hz.hongshengwenyu.top/gtvtxlqfch.html

time ./run.sh
来源：http://hz.ehwqpu.com/gtsmsohhun.html

================================================================================
来源：http://hz.vqdsnc.cn/gtvcmdlhxt.html

S. C / C++ 专题
来源：http://hz.wangshuangyany.cn/gtviuyparl.html

================================================================================
来源：http://hz.yuxming.cn/gtjxpawvak.html

[S01] C：Hello World
来源：http://hz.chenjidiqi.icu/gtvbzozqxr.html

#include <stdio.h>
来源：http://hz.pengpengdd.cyou/gtftuzzauc.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.jiagoushi.top/gtqoiskpma.html

[S02] C：变量与格式化输出
来源：http://hz.chenjidiqi.icu/gtrujodget.html

int a = 10; printf("%d\n", a);
来源：http://hz.shanyushiyangkeji.top/gtzkxomyip.html

[S03] C：读入整数
来源：http://hz.shuidangran.top/gtmkfpmmep.html

int x; scanf("%d", &x);
来源：http://hz.sufxvd.cn/gthmfgxxkf.html

[S04] C：字符串复制
来源：http://hz.sxryk.cn/gtduyvdtsg.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.yuanzhike.top/gtrbcpspux.html

[S05] C：字符串长度
来源：http://hz.hfpthk.cn/gtnxzbrsjz.html

strlen(s)
来源：http://hz.jiagoushi.top/gtnowbthiv.html

[S06] C：字符串比较
来源：http://hz.gotoacloud.top/gtohwsbhqr.html

strcmp(a, b) == 0
来源：http://hz.nanxuanxn.top/gtgkmlhlfq.html

[S07] C：数组遍历求和
来源：http://hz.hongshengwenyu.top/gtuzymzaww.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.ywan-chungtsiang.top/gtdbyugevc.html

[S08] C：动态内存分配与释放
来源：http://hz.daria6918.cn/gtliaabwcr.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.zycfv.cn/gthmmwesho.html

[S09] C：结构体定义与初始化
来源：http://hz.zhiwuduotai.top/gtrgakukff.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.zhengqikj.top/gtsradujne.html

[S10] C：指针与解引用
来源：http://hz.jinghuilouyu.cn/gtgdwrojhs.html

int *p = &a;  *p = 5;
来源：http://hz.yanxiufei.cn/gtjoxolxkm.html

[S11] C：逐行读文件
来源：http://hz.yj20258888.top/gtifevtaqo.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.jqgfzy.top/gtgcilfsrq.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.sxryk.cn/gtktcjiois.html

fclose(f);
来源：http://hz.yonumen.top/gtcfbffqwa.html

[S12] C：写文件
来源：http://hz.havefunace.top/gtdkueafqm.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.zhiwuduotai.top/gtnsuvldbj.html

[S13] C：宏定义
来源：http://hz.yongpay.top/gtqxymlnmg.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.zhiwuduotai.top/gttlhkcybl.html

[S14] C：枚举
来源：http://hz.tanke756.top/gtoouzsxvg.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.smart0.xyz/gtpeaugjfk.html

[S15] C：类型转换
来源：http://hz.hammf.cn/gtgltfalwi.html

(double) a / b
来源：http://hz.shzxlz.cn/gtgerlsotp.html

[S16] C：位操作置位
来源：http://hz.9152youxi.cn/gtmirywkrg.html

x |= (1 << 3);
来源：http://hz.quarkkingdee.top/gtsusobbkl.html

[S17] C：安全拼接字符串
来源：http://hz.dashuyun.cn/gtondtlcdz.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.sweek.top/gtbaezvmym.html

[S18] C：命令行参数
来源：http://hz.iojbl.cn/gtzwydcqsc.html

int main(int argc, char **argv)
来源：http://hz.zhengqikj.top/gtrpfqcwtx.html

[S19] C：快速排序
来源：http://hz.52xcode.cn/gtyaikgfzc.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.yongpay.top/gtufqhxqkm.html

[S20] C：二分查找
来源：http://hz.jqgufenzy.top/gtcimnyssc.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.guowangkeji.top/gtzbatbqne.html

[S21] C：字符类别判断
来源：http://hz.sysykeji.top/gtwluluqmx.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.52xcode.cn/gtzpkuhpnh.html

[S22] C：字符串转数字
来源：http://hz.xinyue.icu/gtkuepxggw.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.vqdsnc.cn/gtfwmtrqim.html

[S23] C：随机数
来源：http://hz.redwolf501.top/gtzljkkouf.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.ybcxt.top/gtanqqdlvg.html

[S24] C：获取本地时间
来源：http://hz.xinyue.icu/gtrdcwvccf.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.jlsjyb.cn/gtfqlxmywy.html

[S25] C：内存拷贝
来源：http://hz.cqqwz.cn/gtnbhjdcuk.html

memcpy(dst, src, n);
来源：http://hz.cdnleiting.top/gtaychnsiq.html

[S26] C：内存清零
来源：http://hz.hammf.cn/gtgxookvcb.html

memset(a, 0, sizeof a);
来源：http://hz.nwbrower.top/gttddcrfdn.html

[S27] C：定义常量
来源：http://hz.gotoacloud.top/gtmnnspruc.html

const double PI = 3.14159;
来源：http://hz.ydzc1.top/gtixsitnmw.html

[S28] C：静态变量
来源：http://hz.jinqigfzy.top/gtgstqaevi.html

static int counter = 0;
来源：http://hz.xylfe.cn/gtehwmyhfj.html

[S29] C：变参函数
来源：http://hz.pengpengdd.cyou/gtmfeykbnx.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.xuanzx.com/gttcgtfgkt.html

[S30] C：头文件保护
来源：http://hz.c1oappe.top/gtuekcaaux.html

#ifndef X_H
来源：http://hz.nanxuanxn.top/gtlvmgjrxk.html

#define X_H
来源：http://hz.xuanzx.com/gtlqcpbvjn.html

#endif
来源：http://hz.sysykeji.top/gtcnvgripa.html

[S31] C++：Hello World
来源：http://hz.aizwys.cn/gtmgaagnep.html

#include <iostream>
来源：http://hz.sweek.top/gtzrjodtdn.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.9152youxi.cn/gtjnbodhow.html

[S32] C++：字符串
来源：http://hz.nanxuanxn.top/gtusrzitsu.html

std::string s = "hi";  s += "!";
来源：http://hz.daria6918.cn/gtwgjgrjwx.html

[S33] C++：vector 增删
来源：http://hz.jiagoushi.top/gtefeszpkv.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.316326.xyz/gtvejvzitl.html

[S34] C++：遍历 vector
来源：http://hz.jqgfzy.top/gtceizyhwl.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.xziqi.cn/gtymbqmpnj.html

[S35] C++：map
来源：http://hz.cucudq.cn/gticuymgvr.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.daria6918.cn/gtbmftklke.html

[S36] C++：unordered_map
来源：http://hz.shangyingyoupin.top/gtjhunlgot.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.ivvv.top/gtqxacaxem.html

[S37] C++：set
来源：http://hz.tianlin.xyz/gtcdvfpkcu.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.shanyushiyangkeji.top/gtyiewbayx.html

[S38] C++：排序
来源：http://hz.c1oappe.top/gtjflkwxpy.html

std::sort(v.begin(), v.end());
来源：http://hz.xingfuxueyuan.xyz/gtssdifhwc.html

[S39] C++：自定义比较器排序
来源：http://hz.yvedp.cn/gtmvlhgvgj.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.nanxuanxn.top/gtbzcnlyff.html

[S40] C++：查找元素
来源：http://hz.daxiang520.top/gtjsyndflh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.vqdsnc.cn/gtoxykhzgg.html

[S41] C++：类与构造函数
来源：http://hz.havefunace.top/gtwjyszeys.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.bjfxy.top/gtpjgmfaoh.html

[S42] C++：继承与虚函数
来源：http://hz.tianlin.xyz/gtxwrzvdme.html

class B : public Base { public: void f() override {} };
来源：http://hz.jlsjyb.cn/gtncdxsblr.html

[S43] C++：智能指针
来源：http://hz.ehwqpu.com/gtjbirrhdn.html

auto p = std::make_unique<int>(5);
来源：http://hz.zhixingplan.top/gtdhzewmkp.html

[S44] C++：引用传参
来源：http://hz.ywan-chungtsiang.top/gtrrsysfre.html

void inc(int &x) { ++x; }
来源：http://hz.sysykeji.top/gtlrkhdvkf.html

[S45] C++：lambda
来源：http://hz.yj202588.top/gtvyxweypd.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.hywenlv.cn/gtpibyzyqu.html

[S46] C++：函数模板
来源：http://hz.ppjwa.cn/gtppukjxhr.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.ehwqpu.com/gtxljimovb.html

[S47] C++：结构化绑定遍历
来源：http://hz.aibaodan.cn/gtvznrlwwi.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.chenjidiqi.icu/gtpuqzcjxt.html

[S48] C++：逐行读文件
来源：http://hz.yongpay.top/gtzopzluiv.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.vqdsnc.cn/gtpyltccnu.html

while (std::getline(in, line)) { }
来源：http://hz.nanxinkj.top/gtckslfwlp.html

[S49] C++：写文件
来源：http://hz.gotoacloud.top/gtfwuowxfe.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.fengsongda.top/gtjfantsws.html

[S50] C++：格式化数字
来源：http://hz.fengsongda.top/gtyxsgkwfr.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.jyoumei.cn/gtsvaphziu.html

[S51] C++：显式类型转换
来源：http://hz.zycfv.cn/gtbiyctsrs.html

static_cast<double>(a) / b
来源：http://hz.zycfv.cn/gtvrunteqa.html

[S52] C++：const 与 noexcept
来源：http://hz.cheryme.top/gtnejvvwbh.html

int size() const noexcept { return n_; }
来源：http://hz.gzhubu.top/gtagzbocat.html

[S53] C++：移动语义
来源：http://hz.nwbrower.top/gtkijmfdpz.html

std::vector<int> w = std::move(v);
来源：http://hz.xziqi.cn/gtklxrmtrj.html

[S54] C++：异常处理
来源：http://hz.hammf.cn/gtdpcyngkq.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.kuanghao11.cn/gtwlhzhjdw.html

[S55] C++：结构化绑定
来源：http://hz.yj202588.top/gtinjmkfvr.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.chenzaomai.com/gtnctgtxgg.html

[S56] C++：optional
来源：http://hz.hfpthk.cn/gteycpzoku.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.gotoacloud.top/gtqbeapqjv.html

[S57] C++：编译期常量
来源：http://hz.tian-w.cn/gtagfwlsvc.html

constexpr int N = 10;
来源：http://hz.nanxuanxn.top/gtysekmitw.html

[S58] C++：命名空间
来源：http://hz.ywan-chungtsiang.top/gtyvyflync.html

namespace ns { int f() { return 1; } }
来源：http://hz.zycfv.cn/gtnszyebpl.html

[S59] C++：静态断言
来源：http://hz.xuanzx.com/gtnnufcbtt.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.xylfe.cn/gtybubvink.html

[S60] C++：遍历并删除元素
来源：http://hz.shanyushiyangkeji.top/gtltzmugti.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.sufxvd.cn/gtptjacazz.html

================================================================================
来源：http://hz.tian-w.cn/gtkaxgzgza.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.ehwqpu.com/gtvqbjuicq.html

================================================================================
来源：http://hz.daria6918.cn/gtstijuzof.html

[T01] Kotlin：Hello World
来源：http://hz.sweek.top/gtynzxsrha.html

println("Hello")
来源：http://hz.dashuyun.cn/gtizqxcuxt.html

[T02] Kotlin：变量
来源：http://hz.yj20258888.top/gtxvetdjxk.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.yanxiufei.cn/gtweqlprzu.html


<!-- 参考信息 -->