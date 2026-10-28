代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.gogol.net.cn/gtsapmoqqi.html

[Q90] 生成序号列
来源：http://hz.aizwys.cn/gtzkdhmjtt.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.cheryme.top/gtlytzvwxv.html

================================================================================
来源：http://hz.xylfe.cn/gtvrrmergi.html

R. Bash 专题
来源：http://hz.xinyue.icu/gtuusnvwks.html

================================================================================
来源：http://hz.yuanzhike.top/gtpzgjoqkv.html

[R01] shebang 与严格模式
来源：http://hz.sufxvd.cn/gtesgkjxsn.html

#!/usr/bin/env bash
来源：http://hz.yonumen.top/gtocosdnya.html

set -euo pipefail
来源：http://hz.zhijiandao.cn/gtonhdayda.html

[R02] 变量赋值与使用
来源：http://hz.jiagoushi.top/gtsoeqhnod.html

name="Tom"; echo "$name"
来源：http://hz.cashguo.top/gtxumayxpg.html

[R03] 只读变量
来源：http://hz.cashguo.top/gthpnszrgw.html

readonly PI=3.14
来源：http://hz.fengsongda.top/gtchfmkpxd.html

[R04] 位置参数
来源：http://hz.wangdashe.top/gtmibtndtd.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.gzhubu.top/gtzccuenkc.html

[R05] 参数默认值
来源：http://hz.haohaochexian.top/gtuqqyiqbc.html

name="${1:-default}"
来源：http://hz.bjfxy.top/gtsgnabsdb.html

[R06] 判断命令是否存在
来源：http://hz.sweek.top/gtlmyzfsga.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.guowangkeji.top/gttenkolqy.html

[R07] if 判断文件
来源：http://hz.andypj.xyz/gttfoqrtfh.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.ppjwa.cn/gtlpzuyjbg.html

[R08] 数值比较
来源：http://hz.zhaomingkeji.xyz/gtawvcppux.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.ppjwa.cn/gtoybzfdso.html

[R09] 字符串比较
来源：http://hz.birdmap.top/gtlnoblmxz.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.xinyue.icu/gtbazlbmuo.html

[R10] 正则匹配
来源：http://hz.yongpay.top/gtttfuxnqe.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.shangyingyoupin.top/gtacgxeulh.html

[R11] case 多分支
来源：http://hz.jinqigfzy.top/gtshvmfeec.html

case "$1" in
来源：http://hz.jinqigfzy.top/gtsboxiikd.html

start) echo "启动" ;;
来源：http://hz.yvedp.cn/gtnxggjpzf.html

stop)  echo "停止" ;;
来源：http://hz.vqdsnc.cn/gtgrvapzax.html

*)     echo "未知命令" ;;
来源：http://hz.guannengcc.top/gtbwwdtijd.html

esac
来源：http://hz.iojbl.cn/gtegdhktrw.html

[R12] for 遍历文件
来源：http://hz.zhixingplan.top/gtftdljpvc.html

for f in *.txt; do echo "$f"; done
来源：http://hz.zhoulong.xyz/gtdwvgynlb.html

[R13] for 计数循环
来源：http://hz.meibo888.top/gtryjsgzpd.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.ppjwa.cn/gtllqdxclz.html

[R14] C 风格 for
来源：http://hz.316326.xyz/gtbtgpxcpr.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.c1oappe.top/gtikvaxzda.html

[R15] while 逐行读文件
来源：http://hz.xylfe.cn/gtkguzuggx.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.xylfe.cn/gtucguayzm.html

[R16] until 等待条件
来源：http://hz.jinyuanbaomall.cn/gtzgveskcx.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.yanxiufei.cn/gtqaainjez.html

[R17] 数组定义与取值
来源：http://hz.yonumen.top/gtlatrqtgj.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.havefunace.top/gtnhgscojj.html

[R18] 遍历数组
来源：http://hz.smart0.xyz/gtynstzrqc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.hammf.cn/gtctnlvbhv.html

[R19] 数组长度
来源：http://hz.yanxiufei.cn/gtbgsbkmhz.html

echo "${#arr[@]}"
来源：http://hz.snrcjt.cn/gtsbdcuzap.html

[R20] 关联数组（字典）
来源：http://hz.xylfe.cn/gtqqfzvred.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.zhoulong.xyz/gtgjykvvou.html

[R21] 字符串长度
来源：http://hz.shuidangran.top/gtmctvrkls.html

echo "${#s}"
来源：http://hz.nanxinkj.top/gtbpjoaspt.html

[R22] 截取子串
来源：http://hz.zycfv.cn/gtlrsoegeu.html

echo "${s:0:5}"
来源：http://hz.redwolf501.top/gtdwfttmic.html

[R23] 字符串替换
来源：http://hz.chenlongwang.top/gtjwtmgzjc.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.zdqjudy.top/gtpzkufqms.html

[R24] 大小写转换
来源：http://hz.pengpengdd.cyou/gtglhkuswa.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.sufxvd.cn/gtkdxusill.html

[R25] 去后缀 / 去前缀
来源：http://hz.xuetiantiany.cn/gtmknjjhrf.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.zhoulong.xyz/gtweumxdgy.html

[R26] 命令替换
来源：http://hz.pengpengdd.cyou/gtodrfjfjd.html

now=$(date +%F); echo "$now"
来源：http://hz.zycfv.cn/gtebodrbte.html

[R27] 算术展开
来源：http://hz.jinghuilouyu.cn/gtpjcbdtiu.html

echo $((1 + 2 * 3))
来源：http://hz.aizwys.cn/gtpeowvbcn.html

[R28] 浮点运算
来源：http://hz.chenlongwang.top/gtsaoawhcz.html

echo "scale=2; 10/3" | bc
来源：http://hz.chenzaomai.com/gtaqymbdse.html

[R29] 定义函数
来源：http://hz.jyoumei.cn/gttsognbkz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.sufxvd.cn/gtrzeuqoap.html

[R30] 函数返回状态码
来源：http://hz.meibo888.top/gtpotbcqui.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.shuidangran.top/gtqhjiuuyw.html

[R31] 局部变量
来源：http://hz.nanxinkj.top/gtqtrhiwsh.html

f() { local x=1; echo "$x"; }
来源：http://hz.zhongyouzk.top/gtokyagxea.html

[R32] 参数个数校验
来源：http://hz.xylfe.cn/gtycpkzhmo.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.jqgufenzy.top/gtdonpxcpj.html

[R33] 捕获错误并提示行号
来源：http://hz.birdmap.top/gtradbwcft.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.tian-w.cn/gtsmgrkzay.html

[R34] 退出时清理
来源：http://hz.vqdsnc.cn/gtfloemoju.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.tianlin.xyz/gtxomtaars.html

[R35] 后台执行并等待
来源：http://hz.shanyushiyangkeji.top/gtxfpxfrpj.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.zhengqikj.top/gtegsrjwwu.html

[R36] 并发执行多个任务
来源：http://hz.nanxuanxn.top/gtducuieqp.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.vqdsnc.cn/gtalnqecge.html

[R37] 把输出赋给变量
来源：http://hz.guowangkeji.top/gtifwxyovr.html

files=$(ls -1)
来源：http://hz.havefunace.top/gtxwueedmp.html

[R38] 管道串联
来源：http://hz.316326.xyz/gtwlpxufeg.html

cat a.txt | grep -i error | wc -l
来源：http://hz.hywenlv.cn/gtuajidxvf.html

[R39] 重定向标准输出与错误
来源：http://hz.zycfv.cn/gthhzwwkaw.html

cmd > out.log 2>&1
来源：http://hz.zhoulong.xyz/gtdypdqtsp.html

[R40] 追加写日志
来源：http://hz.jinghuilouyu.cn/gtcfszuhun.html

echo "log" >> out.log
来源：http://hz.ywan-chungtsiang.top/gteqegxdkl.html

[R41] 丢弃输出
来源：http://hz.yj202588.top/gtassbrlhs.html

cmd >/dev/null 2>&1
来源：http://hz.hysaishi.cn/gtzcbffpcf.html

[R42] 输入重定向
来源：http://hz.0kj1m.cn/gttyrchhur.html

wc -l < a.txt
来源：http://hz.feifeiyinyue.top/gtaotznaqq.html

[R43] 按名字查找文件
来源：http://hz.ydzc1.top/gthhpptkiu.html

find . -name "*.log" -type f
来源：http://hz.0kj1m.cn/gtifbxlaib.html

[R44] 按修改时间查找
来源：http://hz.ppjwa.cn/gtplgzjysw.html

find . -mtime -7 -type f
来源：http://hz.kuanghao11.cn/gtjchacgrz.html

[R45] 批量删除
来源：http://hz.cdnleiting.top/gthsslynkl.html

find . -name "*.tmp" -delete
来源：http://hz.shangyingyoupin.top/gttxugkfut.html

[R46] 递归替换文件内容
来源：http://hz.havefunace.top/gtlvgfgkqv.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.pycfn.com/gtqsrifepg.html

[R47] sed 单行替换
来源：http://hz.gzhubu.top/gtxttinrbg.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.jyoumei.cn/gttzljlojc.html

[R48] awk 取指定列
来源：http://hz.ydjk.org.cn/gtzcwdifnl.html

awk '{print $1, $3}' a.txt
来源：http://hz.meibo888.top/gtizpydfxp.html

[R49] awk 带条件
来源：http://hz.ppjwa.cn/gtrronbbrf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.snrcjt.cn/gtzzgqwjsx.html

[R50] awk 求和
来源：http://hz.meibo888.top/gtmcquyqej.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.yangfankeji.com/gtcwagbbvd.html

[R51] 排序去重取前几
来源：http://hz.dianchejie.cn/gtncrigylm.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.ivvv.top/gtfjmndsep.html

[R52] 统计行数
来源：http://hz.zhijiandao.cn/gtmdzfxyej.html

wc -l a.txt
来源：http://hz.zhaomingkeji.xyz/gtveygtjrm.html

[R53] 查看文件头与实时尾
来源：http://hz.dianchejie.cn/gtrxsmjdnb.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.yonumen.top/gteixnuebt.html

[R54] 比较两个文件
来源：http://hz.aizwys.cn/gtpejdfmlm.html

diff a.txt b.txt
来源：http://hz.9152youxi.cn/gtwdemsuee.html

[R55] 压缩与解压
来源：http://hz.zhiwuduotai.top/gtijjriwfk.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.chenlongwang.top/gtnwrmgveg.html

[R56] 远程拷贝
来源：http://hz.meibo888.top/gtweuwezky.html

scp file user@host:/path/
来源：http://hz.cqqwz.cn/gtqknzcdwc.html

[R57] 远程执行命令
来源：http://hz.tanke756.top/gtgxzhbhkn.html

ssh user@host 'uptime'
来源：http://hz.chenzaomai.com/gthwhvseel.html

[R58] 下载文件
来源：http://hz.pycfn.com/gtitpxdxsy.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.xinyue.icu/gtvdyhvfsn.html

[R59] 发 POST JSON
来源：http://hz.chenjidiqi.icu/gtyiakhsoo.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yonumen.top/gtrppxzeyd.html

[R60] 只看 HTTP 状态码
来源：http://hz.jinqigfzy.top/gtnoaeyavq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.yueranfly.top/gtzlwyhyup.html

[R61] 磁盘占用
来源：http://hz.0kj1m.cn/gtoxopusaz.html

df -h;  du -sh *
来源：http://hz.xylfe.cn/gtthsrckta.html

[R62] 找最占空间的文件
来源：http://hz.chenzaomai.com/gtllpyqwtw.html

du -ah . | sort -rh | head -10
来源：http://hz.smart0.xyz/gteagbvqyx.html

[R63] 内存与进程
来源：http://hz.zhijiandao.cn/gtnzetwhee.html

free -h;  ps aux | grep nginx
来源：http://hz.daxiang520.top/gtoewsbplb.html

[R64] 结束进程
来源：http://hz.pengpengdd.cyou/gttywjcoln.html

kill -9 $(pgrep -f app.py)
来源：http://hz.ybcxt.top/gtshfkpgcg.html

[R65] 查看端口占用
来源：http://hz.yj20258888.top/gtfdnnhiib.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.ivvv.top/gtlnqgnlwp.html

[R66] 定时任务
来源：http://hz.wangshuangyany.cn/gtdafmcwmz.html

crontab -e;  crontab -l
来源：http://hz.hongshengwenyu.top/gtwbetanpa.html

[R67] 生成随机十六进制串
来源：http://hz.andypj.xyz/gtyxzulwaw.html

openssl rand -hex 16
来源：http://hz.fengsongda.top/gtdptwkdts.html

[R68] 计算文件校验值
来源：http://hz.sufxvd.cn/gtibayqoui.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.hfpthk.cn/gtkfoltzta.html

[R69] 生成随机密码
来源：http://hz.chenlongwang.top/gtyntiqbkl.html

head -c 16 /dev/urandom | base64
来源：http://hz.daria6918.cn/gtjuggqzzc.html

[R70] 时间戳与互转
来源：http://hz.c1oappe.top/gteszeqvfj.html

date +%s;  date -d @1700000000
来源：http://hz.vqdsnc.cn/gthsaubjcz.html

[R71] 日期格式化
来源：http://hz.hammf.cn/gtchjklqbu.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.cdnleiting.top/gtpzmzrdqe.html

[R72] 等待端口就绪
来源：http://hz.dashuyun.cn/gtvllojkkx.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.bjfxy.top/gtzquvwsso.html

[R73] 分割大日志
来源：http://hz.nanxinkj.top/gtulxjthbw.html

split -l 1000 big.log part_
来源：http://hz.chenzaomai.com/gtbogyppcd.html

[R74] 批量重命名
来源：http://hz.jinqigufen.top/gtstrpbrkd.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.aibaodan.cn/gtvrppqica.html

[R75] 导出环境变量
来源：http://hz.wangshuangyany.cn/gtmfofydph.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.52xcode.cn/gtzfznfpbv.html

[R76] 使用临时文件
来源：http://hz.316326.xyz/gtbiqgdkfn.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.sysykeji.top/gteluoxkwk.html

[R77] 读取用户输入
来源：http://hz.zhijiandao.cn/gtlqlxqmoj.html

read -rp "请输入: " ans
来源：http://hz.shzxlz.cn/gtvvpggmdm.html

[R78] 交互式菜单
来源：http://hz.cashguo.top/gtufsjweuj.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.mhx1999.top/gtjuiajjrj.html

[R79] 解析命令行选项
来源：http://hz.smart0.xyz/gtegvonnvk.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.guannengcc.top/gtfgpjxsrf.html

[R80] 查看脚本执行耗时
来源：http://hz.fzhhl.top/gthikmvaqz.html

time ./run.sh
来源：http://hz.shanyushiyangtech.top/gtyxnrmyjl.html

================================================================================
来源：http://hz.dashuyun.cn/gtzhygmyvc.html

S. C / C++ 专题
来源：http://hz.cucudq.cn/gtwgpwtphb.html

================================================================================
来源：http://hz.mhx1999.top/gtkwonsuio.html

[S01] C：Hello World
来源：http://hz.tianlin.xyz/gtrbtewqkz.html

#include <stdio.h>
来源：http://hz.gotoacloud.top/gtlnwpxgdx.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.redwolf501.top/gtipmplnod.html

[S02] C：变量与格式化输出
来源：http://hz.yueranfly.top/gtzozlphiy.html

int a = 10; printf("%d\n", a);
来源：http://hz.cashguo.top/gthlcossho.html

[S03] C：读入整数
来源：http://hz.cqqwz.cn/gthtnrdpdj.html

int x; scanf("%d", &x);
来源：http://hz.52xcode.cn/gtetamhrln.html

[S04] C：字符串复制
来源：http://hz.yanxiufei.cn/gttnhhfvwr.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.zycfv.cn/gtqxjwjfnx.html

[S05] C：字符串长度
来源：http://hz.smart0.xyz/gtpdcxuwtx.html

strlen(s)
来源：http://hz.9152youxi.cn/gtszshrujb.html

[S06] C：字符串比较
来源：http://hz.haohaochexian.top/gtzqmrwytz.html

strcmp(a, b) == 0
来源：http://hz.52xcode.cn/gtjmpssmjm.html

[S07] C：数组遍历求和
来源：http://hz.ywan-chungtsiang.top/gtfiwtdfau.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.yangfankeji.com/gtvrchbuep.html

[S08] C：动态内存分配与释放
来源：http://hz.ywan-chungtsiang.top/gtqttmrbxz.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.9152youxi.cn/gtvyjxbzow.html

[S09] C：结构体定义与初始化
来源：http://hz.xylfe.cn/gteyyxuims.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.shzxlz.cn/gtrsqsosel.html

[S10] C：指针与解引用
来源：http://hz.gaohongyu789.top/gtpvyhywvm.html

int *p = &a;  *p = 5;
来源：http://hz.52xcode.cn/gtshnyqreb.html

[S11] C：逐行读文件
来源：http://hz.zdqjudy.top/gturvgeown.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.cheryme.top/gtifvuygue.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.aizwys.cn/gtildggdvu.html

fclose(f);
来源：http://hz.xuanzx.com/gtxlxiuruw.html

[S12] C：写文件
来源：http://hz.gotoacloud.top/gtgzgeqfvk.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.jiagoushi.top/gtyhhbfjjg.html

[S13] C：宏定义
来源：http://hz.tianlin.xyz/gtkervzhad.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.vqdsnc.cn/gthrjlylmq.html

[S14] C：枚举
来源：http://hz.316326.xyz/gthodshmlo.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.9152youxi.cn/gtmgkmlfod.html

[S15] C：类型转换
来源：http://hz.cucudq.cn/gtkyakmykq.html

(double) a / b
来源：http://hz.chenlongwang.top/gtjtjgkxaf.html

[S16] C：位操作置位
来源：http://hz.sxryk.cn/gthnsfrdcc.html

x |= (1 << 3);
来源：http://hz.andypj.xyz/gttrbkxvzm.html

[S17] C：安全拼接字符串
来源：http://hz.yj20258888.top/gtlnrsgnpb.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.tanke756.top/gtnpuubuns.html

[S18] C：命令行参数
来源：http://hz.cucudq.cn/gtviqkhpvu.html

int main(int argc, char **argv)
来源：http://hz.kuanghao11.cn/gtiecdjwmu.html

[S19] C：快速排序
来源：http://hz.gotoacloud.top/gtpklaapig.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.xziqi.cn/gtqwpoczny.html

[S20] C：二分查找
来源：http://hz.jinghuilouyu.cn/gtpqwieifx.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.yvedp.cn/gtuekatwec.html

[S21] C：字符类别判断
来源：http://hz.iojbl.cn/gthanvjnfh.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.yj20258.top/gtrysdpiux.html

[S22] C：字符串转数字
来源：http://hz.aizwys.cn/gtxdxctkem.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.jqgufenzy.top/gtcoaxzpif.html

[S23] C：随机数
来源：http://hz.vqdsnc.cn/gtonqckavy.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.xylfe.cn/gtdpxxnhid.html

[S24] C：获取本地时间
来源：http://hz.chenzaomai.com/gtvtcycxnm.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.hongshengwenyu.top/gtsyjtbkxt.html

[S25] C：内存拷贝
来源：http://hz.nanxuanxn.top/gtvjhijimb.html

memcpy(dst, src, n);
来源：http://hz.jinyuanbaomall.cn/gtssslejdl.html

[S26] C：内存清零
来源：http://hz.yj202588.top/gtciewhudg.html

memset(a, 0, sizeof a);
来源：http://hz.zhijiandao.cn/gtrzlxjlrl.html

[S27] C：定义常量
来源：http://hz.havefunace.top/gtydreaglj.html

const double PI = 3.14159;
来源：http://hz.kuanghao11.cn/gtsuxzuukn.html

[S28] C：静态变量
来源：http://hz.yj20258888.top/gtedcaspgl.html

static int counter = 0;
来源：http://hz.tian-w.cn/gtbwsxitcm.html

[S29] C：变参函数
来源：http://hz.jiagoushi.top/gthqnrztwc.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.jqgufenzy.top/gtbplolnsy.html

[S30] C：头文件保护
来源：http://hz.yueranfly.top/gtofsrrbod.html

#ifndef X_H
来源：http://hz.hnxiangtu.top/gtkfuydewz.html

#define X_H
来源：http://hz.guannengcc.top/gtqwejtixu.html

#endif
来源：http://hz.chenjidiqi.icu/gtwgpevuwm.html

[S31] C++：Hello World
来源：http://hz.yanxiufei.cn/gtimsrpjid.html

#include <iostream>
来源：http://hz.cucudq.cn/gtnclgmaja.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.nanxinkj.top/gtllxntxrq.html

[S32] C++：字符串
来源：http://hz.gzhubu.top/gtgvislwqn.html

std::string s = "hi";  s += "!";
来源：http://hz.fzhhl.top/gtbwdgsbjl.html

[S33] C++：vector 增删
来源：http://hz.dianchejie.cn/gtrhjlayim.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.snrcjt.cn/gtjeovopem.html

[S34] C++：遍历 vector
来源：http://hz.shangyingyoupin.top/gtanluafty.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.fengsongda.top/gtkaabeklg.html

[S35] C++：map
来源：http://hz.jlsjyb.cn/gtjaanxovn.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.sysykeji.top/gtoeyqzskr.html

[S36] C++：unordered_map
来源：http://hz.zhixingplan.top/gtcjxgrjie.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.birdmap.top/gtdvxqtqul.html

[S37] C++：set
来源：http://hz.ywan-chungtsiang.top/gtryaqsqho.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.hfpthk.cn/gtahnkdyne.html

[S38] C++：排序
来源：http://hz.yj20258888.top/gtyqimkfma.html

std::sort(v.begin(), v.end());
来源：http://hz.wangdashe.top/gtjcpmwmvo.html

[S39] C++：自定义比较器排序
来源：http://hz.wangdashe.top/gtzadsgesl.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.gaohongyu789.top/gtpbdkkypp.html

[S40] C++：查找元素
来源：http://hz.pengpengdd.cyou/gtvyxozobu.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.nanxuanxn.top/gtraocdsmr.html

[S41] C++：类与构造函数
来源：http://hz.jqgufenzy.top/gtkpgeughz.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.yj20258888.top/gtogtsetqf.html

[S42] C++：继承与虚函数
来源：http://hz.zhixingplan.top/gtczbimyby.html

class B : public Base { public: void f() override {} };
来源：http://hz.jlsjyb.cn/gthktreuvs.html

[S43] C++：智能指针
来源：http://hz.hnqzz.top/gtssosacjy.html

auto p = std::make_unique<int>(5);
来源：http://hz.yueranfly.top/gtyysbxghk.html

[S44] C++：引用传参
来源：http://hz.ppjwa.cn/gtoqsvyzvh.html

void inc(int &x) { ++x; }
来源：http://hz.c1oappe.top/gtgxrrgnvy.html

[S45] C++：lambda
来源：http://hz.nanxinkj.top/gtsqqpvexl.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.yj20258888.top/gtnrerqthm.html

[S46] C++：函数模板
来源：http://hz.shangyingyoupin.top/gtfpiwcmlc.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.chenzaomai.com/gtspqsumsa.html

[S47] C++：结构化绑定遍历
来源：http://hz.hfpthk.cn/gtsdrskczu.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.guowangkeji.top/gtvxlhoigt.html

[S48] C++：逐行读文件
来源：http://hz.zhoulong.xyz/gtnsirztyn.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.shzxlz.cn/gtaxrcvkiu.html

while (std::getline(in, line)) { }
来源：http://hz.chenjidiqi.icu/gthguzmzma.html

[S49] C++：写文件
来源：http://hz.mhx1999.top/gtfajjsacl.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.hongshengwenyu.top/gtlgpjsyvs.html

[S50] C++：格式化数字
来源：http://hz.ybcxt.top/gtflnqbemv.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.cdnleiting.top/gtkfsfkcby.html

[S51] C++：显式类型转换
来源：http://hz.cqqwz.cn/gtqjunsoul.html

static_cast<double>(a) / b
来源：http://hz.hywenlv.cn/gtbjkbnlwu.html

[S52] C++：const 与 noexcept
来源：http://hz.pycfn.com/gtjijkzefz.html

int size() const noexcept { return n_; }
来源：http://hz.smart0.xyz/gtqledxdow.html

[S53] C++：移动语义
来源：http://hz.hnqzz.top/gtzkmkrbso.html

std::vector<int> w = std::move(v);
来源：http://hz.hongshengwenyu.top/gtbwxidkuu.html

[S54] C++：异常处理
来源：http://hz.shangyingyoupin.top/gtofnftzpt.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.sweek.top/gteffnqpjk.html

[S55] C++：结构化绑定
来源：http://hz.shuidangran.top/gtprnblmot.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.havefunace.top/gtfgzkpxuk.html

[S56] C++：optional
来源：http://hz.yangfankeji.com/gtugjpaxqu.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.zhiwuduotai.top/gthpfcezii.html

[S57] C++：编译期常量
来源：http://hz.ydzc1.top/gtbxnyfjqk.html

constexpr int N = 10;
来源：http://hz.sweek.top/gtrqryydmr.html

[S58] C++：命名空间
来源：http://hz.zhixingplan.top/gtkxmqfhag.html

namespace ns { int f() { return 1; } }
来源：http://hz.cqqwz.cn/gtiyztgaij.html

[S59] C++：静态断言
来源：http://hz.yangfankeji.com/gtymfxskam.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.feifeiyinyue.top/gtyqjuifua.html

[S60] C++：遍历并删除元素
来源：http://hz.ehwqpu.com/gtqsdchger.html


<!-- 参考信息 -->