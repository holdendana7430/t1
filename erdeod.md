代发 wailian999

readonly PI=3.14
来源：http://hz.fengsongda.top/gtugttpleg.html

[R04] 位置参数
来源：http://hz.xuanzx.com/gtlssdvttd.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.zhaomingkeji.xyz/gtssqmowzq.html

[R05] 参数默认值
来源：http://hz.fzhhl.top/gtddiiovih.html

name="${1:-default}"
来源：http://hz.havefunace.top/gtzxysdthc.html

[R06] 判断命令是否存在
来源：http://hz.yj20258888.top/gtpcdhzoig.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.zycfv.cn/gttbgewlpm.html

[R07] if 判断文件
来源：http://hz.jqgfzy.top/gthajcjcow.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.yvedp.cn/gtqhsjrlel.html

[R08] 数值比较
来源：http://hz.cqqwz.cn/gtikrhouwc.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.fzhhl.top/gtpnfvpcoi.html

[R09] 字符串比较
来源：http://hz.nanxinkj.top/gtszpqgyxe.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.yuanzhike.top/gtyzrnbdsu.html

[R10] 正则匹配
来源：http://hz.cheryme.top/gtnsugcvtu.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.fzhhl.top/gtqiohcjer.html

[R11] case 多分支
来源：http://hz.jinyuanbaomall.cn/gtryrqpvcp.html

case "$1" in
来源：http://hz.yj20258.top/gtcwrxrfqh.html

start) echo "启动" ;;
来源：http://hz.yj202588.top/gtfgpxtwpz.html

stop)  echo "停止" ;;
来源：http://hz.jinyuanbaomall.cn/gteluhgqoa.html

*)     echo "未知命令" ;;
来源：http://hz.xuetiantiany.cn/gtpsabjezr.html

esac
来源：http://hz.sufxvd.cn/gtmtzdiwqu.html

[R12] for 遍历文件
来源：http://hz.yj20258888.top/gtbjerefdc.html

for f in *.txt; do echo "$f"; done
来源：http://hz.cheryme.top/gtxlawyuzt.html

[R13] for 计数循环
来源：http://hz.hfpthk.cn/gtdvmxmdke.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.zdqjudy.top/gtxadphxxt.html

[R14] C 风格 for
来源：http://hz.gaohongyu789.top/gttgqtxwvm.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.haohaochexian.top/gtvjnvuruu.html

[R15] while 逐行读文件
来源：http://hz.jianghu66.top/gtrhhapciw.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.sysykeji.top/gtcuibstyk.html

[R16] until 等待条件
来源：http://hz.snrcjt.cn/gtiwwnzycm.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.ivvv.top/gtmcdrqijz.html

[R17] 数组定义与取值
来源：http://hz.pengpengdd.cyou/gtgoeumxhh.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.zhoulong.xyz/gtgmoydhoe.html

[R18] 遍历数组
来源：http://hz.ydjk.org.cn/gtkszjrsyi.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.zhaomingkeji.xyz/gtbdorerac.html

[R19] 数组长度
来源：http://hz.zhaomingkeji.xyz/gtrmactwru.html

echo "${#arr[@]}"
来源：http://hz.shangyingyoupin.top/gttbxdamvv.html

[R20] 关联数组（字典）
来源：http://hz.xuanzx.com/gtltmyfeyo.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.nwbrower.top/gtzkkqtrqq.html

[R21] 字符串长度
来源：http://hz.yanxiufei.cn/gtcnvjfpos.html

echo "${#s}"
来源：http://hz.andypj.xyz/gtnkcjmjtg.html

[R22] 截取子串
来源：http://hz.xuanzx.com/gtxtawxzgv.html

echo "${s:0:5}"
来源：http://hz.yueranfly.top/gtuxfathnc.html

[R23] 字符串替换
来源：http://hz.daria6918.cn/gtfugbkqcq.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.shanyushiyangkeji.top/gtrohngwne.html

[R24] 大小写转换
来源：http://hz.sxryk.cn/gtsgnyxsfa.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.xziqi.cn/gtfrvmuwut.html

[R25] 去后缀 / 去前缀
来源：http://hz.yueranfly.top/gtitawqzkx.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.aibaodan.cn/gttjkghegf.html

[R26] 命令替换
来源：http://hz.sufxvd.cn/gtmthsxrop.html

now=$(date +%F); echo "$now"
来源：http://hz.hongshengwenyu.top/gtoplgftkr.html

[R27] 算术展开
来源：http://hz.zhoulong.xyz/gtsxwpmdui.html

echo $((1 + 2 * 3))
来源：http://hz.yj20258888.top/gtbdkcnorh.html

[R28] 浮点运算
来源：http://hz.cucudq.cn/gtcitjxnjz.html

echo "scale=2; 10/3" | bc
来源：http://hz.wangdashe.top/gtgayfslkg.html

[R29] 定义函数
来源：http://hz.yj202588.top/gtshfervpc.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.yonumen.top/gtjzkmeqbj.html

[R30] 函数返回状态码
来源：http://hz.nanxuanxn.top/gtsnifwvdc.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.zycfv.cn/gtryigjrpt.html

[R31] 局部变量
来源：http://hz.zhoulong.xyz/gtocxwlkbo.html

f() { local x=1; echo "$x"; }
来源：http://hz.hysaishi.cn/gtwepgiacg.html

[R32] 参数个数校验
来源：http://hz.ehwqpu.com/gtiyqtwldz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.0kj1m.cn/gtgcunqdex.html

[R33] 捕获错误并提示行号
来源：http://hz.ywan-chungtsiang.top/gtpwdbteuh.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.sweek.top/gtycugkrxe.html

[R34] 退出时清理
来源：http://hz.ybcxt.top/gtggsnhurk.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.xingfuxueyuan.xyz/gteeauohld.html

[R35] 后台执行并等待
来源：http://hz.zhoulong.xyz/gtmhqxbhua.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.jiagoushi.top/gtuownnfuv.html

[R36] 并发执行多个任务
来源：http://hz.zhengqikj.top/gthgrnbqid.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.zdqjudy.top/gthsukehdk.html

[R37] 把输出赋给变量
来源：http://hz.zhijiandao.cn/gtfcwvkgcj.html

files=$(ls -1)
来源：http://hz.jqgufenzy.top/gtkbwfqfnp.html

[R38] 管道串联
来源：http://hz.hongshengwenyu.top/gtayjkygiq.html

cat a.txt | grep -i error | wc -l
来源：http://hz.yanxiufei.cn/gtebxmgfbx.html

[R39] 重定向标准输出与错误
来源：http://hz.tianlin.xyz/gtiscqgpox.html

cmd > out.log 2>&1
来源：http://hz.feifeiyinyue.top/gteeknsyec.html

[R40] 追加写日志
来源：http://hz.ybcxt.top/gtdqgenbdg.html

echo "log" >> out.log
来源：http://hz.sxryk.cn/gtjnfmjmgx.html

[R41] 丢弃输出
来源：http://hz.ydjk.org.cn/gtvmvpbvjg.html

cmd >/dev/null 2>&1
来源：http://hz.daxiang520.top/gthctfbqar.html

[R42] 输入重定向
来源：http://hz.feifeiyinyue.top/gtjqcnxmve.html

wc -l < a.txt
来源：http://hz.gaohongyu789.top/gtqjexwhow.html

[R43] 按名字查找文件
来源：http://hz.andypj.xyz/gtsqpbvpul.html

find . -name "*.log" -type f
来源：http://hz.yuanzhike.top/gtsbyvoogv.html

[R44] 按修改时间查找
来源：http://hz.xuetiantiany.cn/gtxhfpfnkf.html

find . -mtime -7 -type f
来源：http://hz.sxryk.cn/gtjvxbplva.html

[R45] 批量删除
来源：http://hz.yonumen.top/gtqghqojqo.html

find . -name "*.tmp" -delete
来源：http://hz.zhongyouzk.top/gtamvusdpb.html

[R46] 递归替换文件内容
来源：http://hz.zhiwuduotai.top/gttepzrddk.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.cucudq.cn/gtrysewoxs.html

[R47] sed 单行替换
来源：http://hz.guannengcc.top/gthntqcwse.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.zhaomingkeji.xyz/gtymerdbie.html

[R48] awk 取指定列
来源：http://hz.sufxvd.cn/gtfehaeagv.html

awk '{print $1, $3}' a.txt
来源：http://hz.andypj.xyz/gtdugneetb.html

[R49] awk 带条件
来源：http://hz.xingfuxueyuan.xyz/gtllhvjpuq.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.daxiang520.top/gtisrjlavn.html

[R50] awk 求和
来源：http://hz.ppjwa.cn/gtfxhjfetz.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.zhixingplan.top/gtfnjzedvy.html

[R51] 排序去重取前几
来源：http://hz.gaohongyu789.top/gtsgposklb.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.hysaishi.cn/gtnscgsook.html

[R52] 统计行数
来源：http://hz.ydzc1.top/gtqithdcwg.html

wc -l a.txt
来源：http://hz.zhongyouzk.top/gteiagxkzv.html

[R53] 查看文件头与实时尾
来源：http://hz.svipenyu.cn/gtahkgodls.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.shanyushiyangkeji.top/gtqescigku.html

[R54] 比较两个文件
来源：http://hz.zhixingplan.top/gtprvqdhom.html

diff a.txt b.txt
来源：http://hz.shzxlz.cn/gtjzapvnef.html

[R55] 压缩与解压
来源：http://hz.cashguo.top/gtftvfylsr.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.nanxuanxn.top/gtanulubdp.html

[R56] 远程拷贝
来源：http://hz.xuetiantiany.cn/gthpchuxbc.html

scp file user@host:/path/
来源：http://hz.52xcode.cn/gttyjojlxv.html

[R57] 远程执行命令
来源：http://hz.wangshuangyany.cn/gttsogadgs.html

ssh user@host 'uptime'
来源：http://hz.dashuyun.cn/gtmxkuimha.html

[R58] 下载文件
来源：http://hz.cashguo.top/gtlzfxvrbs.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.9152youxi.cn/gtwqohofhz.html

[R59] 发 POST JSON
来源：http://hz.guowangkeji.top/gtcyoalbvs.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.zhongyouzk.top/gttijqptzy.html

[R60] 只看 HTTP 状态码
来源：http://hz.bjfxy.top/gtgvukavyg.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.smart0.xyz/gtthtpvtmf.html

[R61] 磁盘占用
来源：http://hz.yongpay.top/gtrjezlipz.html

df -h;  du -sh *
来源：http://hz.yonumen.top/gtzfihorrk.html

[R62] 找最占空间的文件
来源：http://hz.daxiang520.top/gtomvpxiyz.html

du -ah . | sort -rh | head -10
来源：http://hz.zycfv.cn/gtjzpfwxbz.html

[R63] 内存与进程
来源：http://hz.fengsongda.top/gtspiazvlt.html

free -h;  ps aux | grep nginx
来源：http://hz.daxiang520.top/gtudoglpxu.html

[R64] 结束进程
来源：http://hz.zhoulong.xyz/gtrxraytvg.html

kill -9 $(pgrep -f app.py)
来源：http://hz.gaohongyu789.top/gtalapqktn.html

[R65] 查看端口占用
来源：http://hz.meibo888.top/gtjdzndlqr.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.yongpay.top/gtyttryaxn.html

[R66] 定时任务
来源：http://hz.fengsongda.top/gtqvxnoeca.html

crontab -e;  crontab -l
来源：http://hz.nanxinkj.top/gtluwbpkqm.html

[R67] 生成随机十六进制串
来源：http://hz.chenjidiqi.icu/gtjzoahbju.html

openssl rand -hex 16
来源：http://hz.jinqigfzy.top/gtkojgzkgy.html

[R68] 计算文件校验值
来源：http://hz.zhijiandao.cn/gtpvnulwpf.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.yj202588.top/gtztpwdtlz.html

[R69] 生成随机密码
来源：http://hz.jyoumei.cn/gtlsechxur.html

head -c 16 /dev/urandom | base64
来源：http://hz.hywenlv.cn/gtvagmargr.html

[R70] 时间戳与互转
来源：http://hz.redwolf501.top/gtgoyjbqlf.html

date +%s;  date -d @1700000000
来源：http://hz.chenzaomai.com/gtufpsfgpn.html

[R71] 日期格式化
来源：http://hz.gotoacloud.top/gtssfgqwmx.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.jianghu66.top/gtnnwzvqlj.html

[R72] 等待端口就绪
来源：http://hz.yuanzhike.top/gtjnsaaiak.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.yuanzhike.top/gtkgrnbsdm.html

[R73] 分割大日志
来源：http://hz.yvedp.cn/gtqitgukgg.html

split -l 1000 big.log part_
来源：http://hz.smart0.xyz/gtkwldkczg.html

[R74] 批量重命名
来源：http://hz.cashguo.top/gtmiqklnsb.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.redwolf501.top/gtlmzgpcjc.html

[R75] 导出环境变量
来源：http://hz.meibo888.top/gtmtkvredq.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.vqdsnc.cn/gtqypltpoh.html

[R76] 使用临时文件
来源：http://hz.havefunace.top/gtmybqbcru.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.ivvv.top/gtwghgfcqm.html

[R77] 读取用户输入
来源：http://hz.nwbrower.top/gtqovpgzra.html

read -rp "请输入: " ans
来源：http://hz.yuanzhike.top/gtjpghorhf.html

[R78] 交互式菜单
来源：http://hz.xingfuxueyuan.xyz/gtcntmcjlu.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.wangdashe.top/gteundhlpc.html

[R79] 解析命令行选项
来源：http://hz.havefunace.top/gtuboiuoqk.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.jqgfzy.top/gtteqgrlwp.html

[R80] 查看脚本执行耗时
来源：http://hz.dashuyun.cn/gtlvswinnf.html

time ./run.sh
来源：http://hz.ppjwa.cn/gtygrbrvql.html

================================================================================
来源：http://hz.haohaochexian.top/gtnfdeyety.html

S. C / C++ 专题
来源：http://hz.chenzaomai.com/gtytmhtmdv.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtgeukqssa.html

[S01] C：Hello World
来源：http://hz.jinyuanbaomall.cn/gtvedbcjfb.html

#include <stdio.h>
来源：http://hz.c1oappe.top/gtywylrzka.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.zhijiandao.cn/gtuqxpypqm.html

[S02] C：变量与格式化输出
来源：http://hz.chenjidiqi.icu/gtmmvkukxz.html

int a = 10; printf("%d\n", a);
来源：http://hz.jqgfzy.top/gtactqljdk.html

[S03] C：读入整数
来源：http://hz.hongshengwenyu.top/gtdtgyyuan.html

int x; scanf("%d", &x);
来源：http://hz.hysaishi.cn/gtcaeivehg.html

[S04] C：字符串复制
来源：http://hz.chenjidiqi.icu/gtxpwpuima.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.yvedp.cn/gtbfpunpxh.html

[S05] C：字符串长度
来源：http://hz.nwbrower.top/gtnsscppqt.html

strlen(s)
来源：http://hz.xylfe.cn/gtwtushzxp.html

[S06] C：字符串比较
来源：http://hz.xuetiantiany.cn/gtrmutqksl.html

strcmp(a, b) == 0
来源：http://hz.havefunace.top/gtjebqlxod.html

[S07] C：数组遍历求和
来源：http://hz.cdnleiting.top/gtnttjjloq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.xziqi.cn/gtdjpnrkqr.html

[S08] C：动态内存分配与释放
来源：http://hz.mhx1999.top/gtuiruyprz.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.daxiang520.top/gtktnetmqq.html

[S09] C：结构体定义与初始化
来源：http://hz.9152youxi.cn/gtjibyapth.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.yuanzhike.top/gtouitrben.html

[S10] C：指针与解引用
来源：http://hz.hywenlv.cn/gtvcojjbbs.html

int *p = &a;  *p = 5;
来源：http://hz.daxiang520.top/gtzgonmocc.html

[S11] C：逐行读文件
来源：http://hz.wangdashe.top/gtydnugkuo.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.yuanzhike.top/gtauviushb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.tianlin.xyz/gtassibfvc.html

fclose(f);
来源：http://hz.yueranfly.top/gthazelecd.html

[S12] C：写文件
来源：http://hz.vqdsnc.cn/gtpqfcgbko.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.aibaodan.cn/gtdzzknyal.html

[S13] C：宏定义
来源：http://hz.chenjidiqi.icu/gtlsvzwmkk.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.jlsjyb.cn/gtjiwgmzpq.html

[S14] C：枚举
来源：http://hz.jinqigufen.top/gtkzvxrfnc.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.jiagoushi.top/gtzvqoeqbn.html

[S15] C：类型转换
来源：http://hz.guannengcc.top/gtqvasktlq.html

(double) a / b
来源：http://hz.wangshuangyany.cn/gtiwkzzzyi.html

[S16] C：位操作置位
来源：http://hz.aizwys.cn/gteeuiauwi.html

x |= (1 << 3);
来源：http://hz.yangfankeji.com/gtekibisxc.html

[S17] C：安全拼接字符串
来源：http://hz.havefunace.top/gtrpxistpl.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.shangyingyoupin.top/gtueefdxoo.html

[S18] C：命令行参数
来源：http://hz.bjfxy.top/gtbrlzdoth.html

int main(int argc, char **argv)
来源：http://hz.ppjwa.cn/gtdbuhprsl.html

[S19] C：快速排序
来源：http://hz.52xcode.cn/gtlyzsrkuq.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.ivvv.top/gtmkrydfpd.html

[S20] C：二分查找
来源：http://hz.yuanzhike.top/gtcohudzrj.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.snrcjt.cn/gtznylwkew.html

[S21] C：字符类别判断
来源：http://hz.yj202588.top/gtzkiqcoar.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.vqdsnc.cn/gthyolsehj.html

[S22] C：字符串转数字
来源：http://hz.aizwys.cn/gtpdmufxqr.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.cqqwz.cn/gtbxrurith.html

[S23] C：随机数
来源：http://hz.xinyue.icu/gtjphimngu.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.sxryk.cn/gtdsdaoinu.html

[S24] C：获取本地时间
来源：http://hz.yuanzhike.top/gtolgucwhh.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.zhixingplan.top/gthyoxbmvh.html

[S25] C：内存拷贝
来源：http://hz.aibaodan.cn/gtftjbwikc.html

memcpy(dst, src, n);
来源：http://hz.chenlongwang.top/gtvflbjsis.html

[S26] C：内存清零
来源：http://hz.cashguo.top/gthbhudzlk.html

memset(a, 0, sizeof a);
来源：http://hz.chenlongwang.top/gttqpboemm.html

[S27] C：定义常量
来源：http://hz.jyoumei.cn/gtwymxwktb.html

const double PI = 3.14159;
来源：http://hz.chenjidiqi.icu/gtqbnrnvcw.html

[S28] C：静态变量
来源：http://hz.yongpay.top/gtyyqcclvi.html

static int counter = 0;
来源：http://hz.cdnleiting.top/gtcpaoztns.html

[S29] C：变参函数
来源：http://hz.jinqigfzy.top/gtrhmfmxef.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.gzhubu.top/gtcueucyar.html

[S30] C：头文件保护
来源：http://hz.gaohongyu789.top/gtojlahlop.html

#ifndef X_H
来源：http://hz.ydzc1.top/gtpgcagelm.html

#define X_H
来源：http://hz.ywan-chungtsiang.top/gtosukalex.html

#endif
来源：http://hz.jinyuanbaomall.cn/gtqkndnbtr.html

[S31] C++：Hello World
来源：http://hz.xylfe.cn/gtuoyyyonl.html

#include <iostream>
来源：http://hz.birdmap.top/gtwkysfjwn.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.svipenyu.cn/gtuvhtwmmr.html

[S32] C++：字符串
来源：http://hz.nanxuanxn.top/gtftjztzyy.html

std::string s = "hi";  s += "!";
来源：http://hz.yj20258.top/gttjfbohdj.html

[S33] C++：vector 增删
来源：http://hz.cheryme.top/gtlvptlgip.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.andypj.xyz/gtrmwqifjt.html

[S34] C++：遍历 vector
来源：http://hz.iojbl.cn/gtfnqllcpk.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.wangdashe.top/gtfajttmmx.html

[S35] C++：map
来源：http://hz.pengpengdd.cyou/gtflumbzxf.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yj20258.top/gtbnwrpgxb.html

[S36] C++：unordered_map
来源：http://hz.zycfv.cn/gtnohbhlra.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.xziqi.cn/gtmhquxrqb.html

[S37] C++：set
来源：http://hz.hywenlv.cn/gtezlnzdjz.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.ppjwa.cn/gtcnrftave.html

[S38] C++：排序
来源：http://hz.tian-w.cn/gtroaclczt.html

std::sort(v.begin(), v.end());
来源：http://hz.birdmap.top/gtjaurgdqy.html

[S39] C++：自定义比较器排序
来源：http://hz.gaohongyu789.top/gtmomrngdl.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.gzhubu.top/gtnskvpoce.html

[S40] C++：查找元素
来源：http://hz.nanxuanxn.top/gtckkmdnjn.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.zhijiandao.cn/gtvjwedwtm.html

[S41] C++：类与构造函数
来源：http://hz.redwolf501.top/gtohjxblps.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.hysaishi.cn/gtoeityqzy.html

[S42] C++：继承与虚函数
来源：http://hz.yvedp.cn/gtfxdlxtze.html

class B : public Base { public: void f() override {} };
来源：http://hz.dashuyun.cn/gtuuzxmisw.html

[S43] C++：智能指针
来源：http://hz.jqgfzy.top/gtmuzplwfp.html

auto p = std::make_unique<int>(5);
来源：http://hz.dashuyun.cn/gtmazlkglj.html

[S44] C++：引用传参
来源：http://hz.bjfxy.top/gtoovtvtjc.html

void inc(int &x) { ++x; }
来源：http://hz.dianchejie.cn/gtipmuwfsd.html

[S45] C++：lambda
来源：http://hz.xuanzx.com/gtrgfgdmyi.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.hywenlv.cn/gtxdvcxktg.html

[S46] C++：函数模板
来源：http://hz.aizwys.cn/gtgawqdvbz.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.fzhhl.top/gtvvdpoocw.html

[S47] C++：结构化绑定遍历
来源：http://hz.jinqigufen.top/gttnqwrytt.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.tanke756.top/gtxbadospl.html

[S48] C++：逐行读文件
来源：http://hz.snrcjt.cn/gtsaydiczg.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.gaohongyu789.top/gtkjabsice.html

while (std::getline(in, line)) { }
来源：http://hz.shangyingyoupin.top/gtzezyoege.html

[S49] C++：写文件
来源：http://hz.hnqzz.top/gtacpcbzty.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.hnqzz.top/gtiimosgts.html

[S50] C++：格式化数字
来源：http://hz.ehwqpu.com/gtxlcembdm.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.zhongyouzk.top/gtutcknmji.html

[S51] C++：显式类型转换
来源：http://hz.ywan-chungtsiang.top/gtnuqlufvd.html

static_cast<double>(a) / b
来源：http://hz.cdnleiting.top/gturnwnnrg.html

[S52] C++：const 与 noexcept
来源：http://hz.tanke756.top/gtvlknbsnu.html

int size() const noexcept { return n_; }
来源：http://hz.hongshengwenyu.top/gtknmshttb.html

[S53] C++：移动语义
来源：http://hz.kuanghao11.cn/gtxqktznrt.html

std::vector<int> w = std::move(v);
来源：http://hz.xuanzx.com/gtacdrufoo.html

[S54] C++：异常处理
来源：http://hz.zdqjudy.top/gtahggokvp.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.yuxming.cn/gteywiceun.html

[S55] C++：结构化绑定
来源：http://hz.sweek.top/gtherlkylr.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.mhx1999.top/gttifffdcj.html

[S56] C++：optional
来源：http://hz.nanxuanxn.top/gtnqnzegls.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.hnqzz.top/gtalconmlb.html

[S57] C++：编译期常量
来源：http://hz.yangfankeji.com/gtszmkdhdq.html

constexpr int N = 10;
来源：http://hz.zhixingplan.top/gtrmxwptne.html

[S58] C++：命名空间
来源：http://hz.yvedp.cn/gtuzyyjugk.html

namespace ns { int f() { return 1; } }
来源：http://hz.birdmap.top/gtttuhfdaq.html

[S59] C++：静态断言
来源：http://hz.aizwys.cn/gtbqvxmgaw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.yanxiufei.cn/gtpjibbjah.html

[S60] C++：遍历并删除元素
来源：http://hz.shanyushiyangkeji.top/gtdwdbgmgr.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.haohaochexian.top/gtcxbbqeuf.html

================================================================================
来源：http://hz.jiagoushi.top/gtaktzazqz.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.dashuyun.cn/gtbhseavnh.html

================================================================================
来源：http://hz.mhx1999.top/gtnkujtgax.html

[T01] Kotlin：Hello World
来源：http://hz.gaohongyu789.top/gtwiklgrmz.html

println("Hello")
来源：http://hz.gogol.net.cn/gttropjqwz.html

[T02] Kotlin：变量
来源：http://hz.zhongyouzk.top/gtulumxykg.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.zhixingplan.top/gtlbsiehdf.html

[T03] Kotlin：字符串模板
来源：http://hz.smart0.xyz/gtixwputsj.html

"值: $b"
来源：http://hz.havefunace.top/gtuqddjalp.html

[T04] Kotlin：空安全
来源：http://hz.xziqi.cn/gtclriqjyr.html

val n: String? = null;  n?.length
来源：http://hz.hysaishi.cn/gtzujizlhc.html


<!-- 参考信息 -->