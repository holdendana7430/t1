代发 wailian999

set -euo pipefail
来源：http://hz.sxryk.cn/gtwpqbbjht.html

[R02] 变量赋值与使用
来源：http://hz.snrcjt.cn/gtxcxvuyph.html

name="Tom"; echo "$name"
来源：http://hz.0kj1m.cn/gtjovofqoc.html

[R03] 只读变量
来源：http://hz.smart0.xyz/gtbjtrkiew.html

readonly PI=3.14
来源：http://hz.jlsjyb.cn/gtkwxngtbm.html

[R04] 位置参数
来源：http://hz.316326.xyz/gttpckunfs.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.xingfuxueyuan.xyz/gtspdvkkbe.html

[R05] 参数默认值
来源：http://hz.birdmap.top/gtuzvgycpc.html

name="${1:-default}"
来源：http://hz.cheryme.top/gtmqpiibzb.html

[R06] 判断命令是否存在
来源：http://hz.zhoulong.xyz/gtcghymipc.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.ywan-chungtsiang.top/gtvfnkbaby.html

[R07] if 判断文件
来源：http://hz.c1oappe.top/gtkexlxtjb.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.ivvv.top/gtubxnpzva.html

[R08] 数值比较
来源：http://hz.yuxming.cn/gtxsshaboa.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.kuanghao11.cn/gtgiwawxzd.html

[R09] 字符串比较
来源：http://hz.havefunace.top/gtfkaqqonx.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.yvedp.cn/gtftvprlgp.html

[R10] 正则匹配
来源：http://hz.9152youxi.cn/gtpmknahmb.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.pengpengdd.cyou/gtfqilxxef.html

[R11] case 多分支
来源：http://hz.cheryme.top/gtcbnbotap.html

case "$1" in
来源：http://hz.chenlongwang.top/gtvriwifgp.html

start) echo "启动" ;;
来源：http://hz.yanxiufei.cn/gtmebrrnha.html

stop)  echo "停止" ;;
来源：http://hz.hnqzz.top/gtpzlfwihz.html

*)     echo "未知命令" ;;
来源：http://hz.xuetiantiany.cn/gtgpwpoaki.html

esac
来源：http://hz.jlsjyb.cn/gtvwratbnb.html

[R12] for 遍历文件
来源：http://hz.xuanzx.com/gtihvocxqe.html

for f in *.txt; do echo "$f"; done
来源：http://hz.jlsjyb.cn/gtgrezipsb.html

[R13] for 计数循环
来源：http://hz.chenjidiqi.icu/gtksmqeqvp.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.zdqjudy.top/gtxnjfxhdy.html

[R14] C 风格 for
来源：http://hz.pengpengdd.cyou/gtjmnfbgcd.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.hnqzz.top/gtvcudfpkz.html

[R15] while 逐行读文件
来源：http://hz.redwolf501.top/gthrhbjbax.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.havefunace.top/gtroqjsaqy.html

[R16] until 等待条件
来源：http://hz.zhengqikj.top/gtauhczbtl.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.aibaodan.cn/gtyegxmpkl.html

[R17] 数组定义与取值
来源：http://hz.snrcjt.cn/gtopqlknat.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.jlsjyb.cn/gtsahdtott.html

[R18] 遍历数组
来源：http://hz.zhongyouzk.top/gtqdnxsrls.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.shanyushiyangtech.top/gtcahrnycs.html

[R19] 数组长度
来源：http://hz.guannengcc.top/gtkiroozlm.html

echo "${#arr[@]}"
来源：http://hz.snrcjt.cn/gtsegybpnc.html

[R20] 关联数组（字典）
来源：http://hz.haohaochexian.top/gtzdlkexva.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.zhongyouzk.top/gtcwkvjbtl.html

[R21] 字符串长度
来源：http://hz.shuidangran.top/gtkwpxwuxc.html

echo "${#s}"
来源：http://hz.jyoumei.cn/gtnryicqea.html

[R22] 截取子串
来源：http://hz.yonumen.top/gttuvljvnb.html

echo "${s:0:5}"
来源：http://hz.daxiang520.top/gtiecikirg.html

[R23] 字符串替换
来源：http://hz.xinyue.icu/gtxycuqjgp.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.jinqigfzy.top/gtzawmmtbg.html

[R24] 大小写转换
来源：http://hz.hammf.cn/gtuaclamye.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.ydjk.org.cn/gtkzxcrhnb.html

[R25] 去后缀 / 去前缀
来源：http://hz.gogol.net.cn/gtikfcrddf.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.c1oappe.top/gtwpfqqusd.html

[R26] 命令替换
来源：http://hz.cdnleiting.top/gtimyloswv.html

now=$(date +%F); echo "$now"
来源：http://hz.sufxvd.cn/gtjakqsrfr.html

[R27] 算术展开
来源：http://hz.sweek.top/gtekgacjup.html

echo $((1 + 2 * 3))
来源：http://hz.hammf.cn/gtdyvqjucs.html

[R28] 浮点运算
来源：http://hz.dashuyun.cn/gtelwculcp.html

echo "scale=2; 10/3" | bc
来源：http://hz.gotoacloud.top/gtylkngcbr.html

[R29] 定义函数
来源：http://hz.xziqi.cn/gtqnltzuqq.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.jlsjyb.cn/gtoooxitjc.html

[R30] 函数返回状态码
来源：http://hz.pengpengdd.cyou/gtubxasmhz.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.nanxuanxn.top/gtnsueasaw.html

[R31] 局部变量
来源：http://hz.jinqigufen.top/gttfxqxlfr.html

f() { local x=1; echo "$x"; }
来源：http://hz.fengsongda.top/gtrwfuqjpd.html

[R32] 参数个数校验
来源：http://hz.daria6918.cn/gtnvklkepl.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.0kj1m.cn/gtzwpiszkl.html

[R33] 捕获错误并提示行号
来源：http://hz.tianlin.xyz/gtytnpntdf.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.gzhubu.top/gtzqcigqrn.html

[R34] 退出时清理
来源：http://hz.zhoulong.xyz/gtdnratskb.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.chenzaomai.com/gtodcmkuly.html

[R35] 后台执行并等待
来源：http://hz.feifeiyinyue.top/gtlpqtbult.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.yuxming.cn/gtoyaqhstu.html

[R36] 并发执行多个任务
来源：http://hz.aibaodan.cn/gtfzjqzxzd.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.fengsongda.top/gtmlbkhpup.html

[R37] 把输出赋给变量
来源：http://hz.aibaodan.cn/gtilfafbwz.html

files=$(ls -1)
来源：http://hz.mhx1999.top/gtkxjveetc.html

[R38] 管道串联
来源：http://hz.9152youxi.cn/gtedgrboug.html

cat a.txt | grep -i error | wc -l
来源：http://hz.xinyue.icu/gtzmmerdpw.html

[R39] 重定向标准输出与错误
来源：http://hz.jlsjyb.cn/gtmymimiak.html

cmd > out.log 2>&1
来源：http://hz.gogol.net.cn/gtrsrejryc.html

[R40] 追加写日志
来源：http://hz.yuxming.cn/gtpipjmfkb.html

echo "log" >> out.log
来源：http://hz.quarkkingdee.top/gtsrlcflbx.html

[R41] 丢弃输出
来源：http://hz.chenlongwang.top/gtfjnrstmt.html

cmd >/dev/null 2>&1
来源：http://hz.hongshengwenyu.top/gtcbeyytgk.html

[R42] 输入重定向
来源：http://hz.9152youxi.cn/gttvmzgqms.html

wc -l < a.txt
来源：http://hz.yongpay.top/gtbaslwsbf.html

[R43] 按名字查找文件
来源：http://hz.jyoumei.cn/gtfyrpukcq.html

find . -name "*.log" -type f
来源：http://hz.jinghuilouyu.cn/gtycqcmttz.html

[R44] 按修改时间查找
来源：http://hz.zhongyouzk.top/gtgvtnlwwe.html

find . -mtime -7 -type f
来源：http://hz.zhongyouzk.top/gtzoufyxdm.html

[R45] 批量删除
来源：http://hz.wangshuangyany.cn/gtaxqzyahq.html

find . -name "*.tmp" -delete
来源：http://hz.bjfxy.top/gtnoibengq.html

[R46] 递归替换文件内容
来源：http://hz.ppjwa.cn/gtgesibakq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.cqqwz.cn/gtimmittgl.html

[R47] sed 单行替换
来源：http://hz.wangshuangyany.cn/gtnnrxjwsn.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.hywenlv.cn/gtvtiixlms.html

[R48] awk 取指定列
来源：http://hz.cheryme.top/gtfnkwzdib.html

awk '{print $1, $3}' a.txt
来源：http://hz.zhaomingkeji.xyz/gtflxeyehn.html

[R49] awk 带条件
来源：http://hz.ybcxt.top/gtnzoilbfq.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.ehwqpu.com/gtpptxjxkh.html

[R50] awk 求和
来源：http://hz.c1oappe.top/gtvnlxrwpq.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.meibo888.top/gtzlqppvcf.html

[R51] 排序去重取前几
来源：http://hz.dashuyun.cn/gtqahfkvsy.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.cashguo.top/gtewkkyang.html

[R52] 统计行数
来源：http://hz.nwbrower.top/gtvxbwoghs.html

wc -l a.txt
来源：http://hz.jinqigfzy.top/gtjlhinoxn.html

[R53] 查看文件头与实时尾
来源：http://hz.ppjwa.cn/gtfasicpad.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.havefunace.top/gtaxyefaqy.html

[R54] 比较两个文件
来源：http://hz.hnxiangtu.top/gtocttfxuc.html

diff a.txt b.txt
来源：http://hz.shzxlz.cn/gtmlnugwgl.html

[R55] 压缩与解压
来源：http://hz.wangshuangyany.cn/gtoigbgtft.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.xuanzx.com/gtcjpcmqbt.html

[R56] 远程拷贝
来源：http://hz.smart0.xyz/gtaixeubun.html

scp file user@host:/path/
来源：http://hz.meibo888.top/gtwavadnfk.html

[R57] 远程执行命令
来源：http://hz.fzhhl.top/gteqervrxi.html

ssh user@host 'uptime'
来源：http://hz.svipenyu.cn/gtshcaouyx.html

[R58] 下载文件
来源：http://hz.shanyushiyangkeji.top/gtatrxwfim.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.dashuyun.cn/gtcgoxccrc.html

[R59] 发 POST JSON
来源：http://hz.hnqzz.top/gtmionfasf.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.9152youxi.cn/gtvbswbbzq.html

[R60] 只看 HTTP 状态码
来源：http://hz.havefunace.top/gtkoonwxcq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.daxiang520.top/gtbujzbtua.html

[R61] 磁盘占用
来源：http://hz.xylfe.cn/gtcxdtbpop.html

df -h;  du -sh *
来源：http://hz.yj202588.top/gtyehscddb.html

[R62] 找最占空间的文件
来源：http://hz.zhixingplan.top/gtpcejwhru.html

du -ah . | sort -rh | head -10
来源：http://hz.feifeiyinyue.top/gtsiflkkdw.html

[R63] 内存与进程
来源：http://hz.sufxvd.cn/gtninriwkv.html

free -h;  ps aux | grep nginx
来源：http://hz.yuanzhike.top/gtdtkohcsc.html

[R64] 结束进程
来源：http://hz.gotoacloud.top/gtbewdrouy.html

kill -9 $(pgrep -f app.py)
来源：http://hz.xinyue.icu/gtxaejtfgs.html

[R65] 查看端口占用
来源：http://hz.jyoumei.cn/gtammrewia.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.zhaomingkeji.xyz/gtqkksccna.html

[R66] 定时任务
来源：http://hz.chenlongwang.top/gtckjovhwi.html

crontab -e;  crontab -l
来源：http://hz.jiagoushi.top/gtjwmbbqgs.html

[R67] 生成随机十六进制串
来源：http://hz.hnqzz.top/gtdhpgduha.html

openssl rand -hex 16
来源：http://hz.snrcjt.cn/gtduggokgx.html

[R68] 计算文件校验值
来源：http://hz.gogol.net.cn/gtzpeteosd.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.zhengqikj.top/gtkcfncxpk.html

[R69] 生成随机密码
来源：http://hz.gaohongyu789.top/gtyhkntren.html

head -c 16 /dev/urandom | base64
来源：http://hz.chenlongwang.top/gtfeqwqaki.html

[R70] 时间戳与互转
来源：http://hz.52xcode.cn/gtyanwgmqt.html

date +%s;  date -d @1700000000
来源：http://hz.haohaochexian.top/gtrevgffvt.html

[R71] 日期格式化
来源：http://hz.yueranfly.top/gtbpvriqln.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.ywan-chungtsiang.top/gtzpjjbkmb.html

[R72] 等待端口就绪
来源：http://hz.gotoacloud.top/gtvtjlqgnf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.ybcxt.top/gtytidpkvg.html

[R73] 分割大日志
来源：http://hz.xylfe.cn/gtankbibbl.html

split -l 1000 big.log part_
来源：http://hz.tianlin.xyz/gtywsyimmy.html

[R74] 批量重命名
来源：http://hz.tian-w.cn/gtislcnbfc.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.zhixingplan.top/gtjdcemzqh.html

[R75] 导出环境变量
来源：http://hz.svipenyu.cn/gtnfbiofsd.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.zdqjudy.top/gttoarmomq.html

[R76] 使用临时文件
来源：http://hz.nwbrower.top/gtzveqbxmh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.xuetiantiany.cn/gtdtskjhjp.html

[R77] 读取用户输入
来源：http://hz.0kj1m.cn/gtlqsegeib.html

read -rp "请输入: " ans
来源：http://hz.yj20258888.top/gtuzofrgtc.html

[R78] 交互式菜单
来源：http://hz.9152youxi.cn/gttnmhzusg.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.daxiang520.top/gtexrrxgzs.html

[R79] 解析命令行选项
来源：http://hz.andypj.xyz/gteaxoembu.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.yongpay.top/gtevcdzygk.html

[R80] 查看脚本执行耗时
来源：http://hz.yuanzhike.top/gtmokpqxen.html

time ./run.sh
来源：http://hz.nanxuanxn.top/gtmneiksok.html

================================================================================
来源：http://hz.svipenyu.cn/gtaxgwriuw.html

S. C / C++ 专题
来源：http://hz.zycfv.cn/gtdfkhwhij.html

================================================================================
来源：http://hz.dianchejie.cn/gtpevplpgo.html

[S01] C：Hello World
来源：http://hz.wangshuangyany.cn/gtzbanmtqq.html

#include <stdio.h>
来源：http://hz.ydzc1.top/gtroliiuwy.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.pycfn.com/gtqudgqjpy.html

[S02] C：变量与格式化输出
来源：http://hz.pycfn.com/gtpdezbojt.html

int a = 10; printf("%d\n", a);
来源：http://hz.guowangkeji.top/gthttiztrd.html

[S03] C：读入整数
来源：http://hz.ivvv.top/gtfytjjfpe.html

int x; scanf("%d", &x);
来源：http://hz.cdnleiting.top/gttquyjvtc.html

[S04] C：字符串复制
来源：http://hz.cheryme.top/gtgkuskzfm.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.gotoacloud.top/gtbjoeccjm.html

[S05] C：字符串长度
来源：http://hz.smart0.xyz/gtiuxcsgdx.html

strlen(s)
来源：http://hz.pycfn.com/gtyjunybfr.html

[S06] C：字符串比较
来源：http://hz.mhx1999.top/gtwdtkcdck.html

strcmp(a, b) == 0
来源：http://hz.yongpay.top/gtwemgtmjd.html

[S07] C：数组遍历求和
来源：http://hz.yanxiufei.cn/gttwobkjza.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.xziqi.cn/gtnvvbxnjv.html

[S08] C：动态内存分配与释放
来源：http://hz.daria6918.cn/gtbxogogux.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.jinqigfzy.top/gtlwxyuzkf.html

[S09] C：结构体定义与初始化
来源：http://hz.xingfuxueyuan.xyz/gtldhsdbxw.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.bjfxy.top/gtyndoaqam.html

[S10] C：指针与解引用
来源：http://hz.xingfuxueyuan.xyz/gtjxaucvlr.html

int *p = &a;  *p = 5;
来源：http://hz.havefunace.top/gtwskkozuf.html

[S11] C：逐行读文件
来源：http://hz.chenzaomai.com/gtvxgyqgqn.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.shangyingyoupin.top/gtwbrrdwfu.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.mhx1999.top/gtjmxgikfh.html

fclose(f);
来源：http://hz.gzhubu.top/gtkdyaqmey.html

[S12] C：写文件
来源：http://hz.sysykeji.top/gtykkyktxh.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.zdqjudy.top/gtsxhvcpna.html

[S13] C：宏定义
来源：http://hz.xziqi.cn/gtgugiaxdf.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.yongpay.top/gtlrrenuag.html

[S14] C：枚举
来源：http://hz.yueranfly.top/gtxfzjbfbf.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.jinghuilouyu.cn/gtpciseqbu.html

[S15] C：类型转换
来源：http://hz.havefunace.top/gtbpbcgupp.html

(double) a / b
来源：http://hz.yonumen.top/gtbtboiyer.html

[S16] C：位操作置位
来源：http://hz.nanxuanxn.top/gtzjdafdem.html

x |= (1 << 3);
来源：http://hz.dashuyun.cn/gtaqgghipz.html

[S17] C：安全拼接字符串
来源：http://hz.xinyue.icu/gtzyenbide.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.shanyushiyangtech.top/gtarvjpngy.html

[S18] C：命令行参数
来源：http://hz.yongpay.top/gtnibpkoxl.html

int main(int argc, char **argv)
来源：http://hz.yj20258.top/gtvcqjcrju.html

[S19] C：快速排序
来源：http://hz.jinqigfzy.top/gtbjcnfsnt.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.jinqigfzy.top/gtefpzoryl.html

[S20] C：二分查找
来源：http://hz.gaohongyu789.top/gtsikwqhjg.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.smart0.xyz/gtuwlirxzb.html

[S21] C：字符类别判断
来源：http://hz.jiagoushi.top/gtvccuwysr.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.xinyue.icu/gtyqfqxmyk.html

[S22] C：字符串转数字
来源：http://hz.hywenlv.cn/gtkcbpbfdv.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.zhijiandao.cn/gtxpfwtwgv.html

[S23] C：随机数
来源：http://hz.chenlongwang.top/gthsyquhyz.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.gotoacloud.top/gtuzaadpiu.html

[S24] C：获取本地时间
来源：http://hz.hnxiangtu.top/gtxjjumydn.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.jinqigfzy.top/gtqiydfckx.html

[S25] C：内存拷贝
来源：http://hz.hywenlv.cn/gtggbjfnjk.html

memcpy(dst, src, n);
来源：http://hz.jinyuanbaomall.cn/gtvtwwctrp.html

[S26] C：内存清零
来源：http://hz.ybcxt.top/gtuuelkfsf.html

memset(a, 0, sizeof a);
来源：http://hz.c1oappe.top/gtjrefczav.html

[S27] C：定义常量
来源：http://hz.pycfn.com/gtpibgygto.html

const double PI = 3.14159;
来源：http://hz.cashguo.top/gtivrwxzuu.html

[S28] C：静态变量
来源：http://hz.zhaomingkeji.xyz/gtzowjithe.html

static int counter = 0;
来源：http://hz.chenzaomai.com/gtasxuuxla.html

[S29] C：变参函数
来源：http://hz.316326.xyz/gtoggakqio.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.sysykeji.top/gtngltrovc.html

[S30] C：头文件保护
来源：http://hz.0kj1m.cn/gtlxzyezmy.html

#ifndef X_H
来源：http://hz.ydjk.org.cn/gtyapzrrgl.html

#define X_H
来源：http://hz.hongshengwenyu.top/gtgtvqcmhq.html

#endif
来源：http://hz.xuetiantiany.cn/gtebpufgyk.html

[S31] C++：Hello World
来源：http://hz.nanxuanxn.top/gtzpixnsii.html

#include <iostream>
来源：http://hz.ehwqpu.com/gtgcmntgnu.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.zhixingplan.top/gtnjlhbyfp.html

[S32] C++：字符串
来源：http://hz.52xcode.cn/gtshmthaih.html

std::string s = "hi";  s += "!";
来源：http://hz.zhixingplan.top/gtulndeyih.html

[S33] C++：vector 增删
来源：http://hz.xuetiantiany.cn/gtubvdonio.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.sxryk.cn/gtfwgkjydm.html

[S34] C++：遍历 vector
来源：http://hz.xuetiantiany.cn/gtgwhhnpkd.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.svipenyu.cn/gtkbzfrxee.html

[S35] C++：map
来源：http://hz.tanke756.top/gtiiqgpyhy.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.sysykeji.top/gthjlnpadl.html

[S36] C++：unordered_map
来源：http://hz.jlsjyb.cn/gtwrzdpqsb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jiagoushi.top/gtlkcipnpe.html

[S37] C++：set
来源：http://hz.zycfv.cn/gtitpgmmfv.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.cucudq.cn/gtitlvxphi.html

[S38] C++：排序
来源：http://hz.yvedp.cn/gtufzngppt.html

std::sort(v.begin(), v.end());
来源：http://hz.haohaochexian.top/gtbassujlk.html

[S39] C++：自定义比较器排序
来源：http://hz.52xcode.cn/gtbxirwhgz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.gaohongyu789.top/gtmduapzqr.html

[S40] C++：查找元素
来源：http://hz.fengsongda.top/gtbanbirom.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.xuetiantiany.cn/gtadluxhdx.html

[S41] C++：类与构造函数
来源：http://hz.hnqzz.top/gtmdvjsrxx.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.yj20258888.top/gtptvqcaun.html

[S42] C++：继承与虚函数
来源：http://hz.gaohongyu789.top/gtgwmbviwl.html

class B : public Base { public: void f() override {} };
来源：http://hz.hnxiangtu.top/gtsfkatikt.html

[S43] C++：智能指针
来源：http://hz.ehwqpu.com/gtmjpvnymd.html

auto p = std::make_unique<int>(5);
来源：http://hz.cashguo.top/gtibtczxcr.html

[S44] C++：引用传参
来源：http://hz.c1oappe.top/gtzcrzgred.html

void inc(int &x) { ++x; }
来源：http://hz.zhiwuduotai.top/gtimpuncms.html

[S45] C++：lambda
来源：http://hz.sxryk.cn/gtrspifvym.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.sweek.top/gtekqklwuw.html

[S46] C++：函数模板
来源：http://hz.yj202588.top/gtjqojkgxy.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.hongshengwenyu.top/gttxwhzffd.html

[S47] C++：结构化绑定遍历
来源：http://hz.smart0.xyz/gtnmcqxcax.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.yongpay.top/gtdwwnhwjx.html

[S48] C++：逐行读文件
来源：http://hz.jyoumei.cn/gtmcyezvis.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.quarkkingdee.top/gtmrocptjx.html

while (std::getline(in, line)) { }
来源：http://hz.cheryme.top/gtwtfizyyw.html

[S49] C++：写文件
来源：http://hz.tanke756.top/gtqftdnnzx.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.hnqzz.top/gtjgcwstrx.html

[S50] C++：格式化数字
来源：http://hz.nanxinkj.top/gtmxaxztvo.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.jyoumei.cn/gtbugcjsst.html

[S51] C++：显式类型转换
来源：http://hz.cheryme.top/gtopvljszy.html

static_cast<double>(a) / b
来源：http://hz.hysaishi.cn/gtjuhfitdt.html

[S52] C++：const 与 noexcept
来源：http://hz.quarkkingdee.top/gtkvacoeab.html

int size() const noexcept { return n_; }
来源：http://hz.yj20258888.top/gtbwzhrlrj.html

[S53] C++：移动语义
来源：http://hz.ybcxt.top/gtwryeravj.html

std::vector<int> w = std::move(v);
来源：http://hz.sweek.top/gtopsethsl.html

[S54] C++：异常处理
来源：http://hz.hnqzz.top/gtahlrqqet.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.fzhhl.top/gtnqkyanvl.html

[S55] C++：结构化绑定
来源：http://hz.bjfxy.top/gtwfklutbx.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.yj20258.top/gtjqyozzbo.html

[S56] C++：optional
来源：http://hz.hammf.cn/gtmnrvrcbi.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.aizwys.cn/gtozrkrlrf.html

[S57] C++：编译期常量
来源：http://hz.quarkkingdee.top/gtzmhwnjvm.html

constexpr int N = 10;
来源：http://hz.ywan-chungtsiang.top/gtedgpjzer.html

[S58] C++：命名空间
来源：http://hz.shuidangran.top/gthtycvyrw.html

namespace ns { int f() { return 1; } }
来源：http://hz.hywenlv.cn/gtcjqgcstz.html

[S59] C++：静态断言
来源：http://hz.shangyingyoupin.top/gtccfholsl.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.gaohongyu789.top/gtyawcgjzs.html

[S60] C++：遍历并删除元素
来源：http://hz.xuetiantiany.cn/gtiirxsrwp.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.cheryme.top/gtkmtrixej.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtbgrjcugc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.ivvv.top/gtjemijjqs.html

================================================================================
来源：http://hz.yanxiufei.cn/gtcvyyeqcc.html

[T01] Kotlin：Hello World
来源：http://hz.wangshuangyany.cn/gtemsbgeon.html

println("Hello")
来源：http://hz.sxryk.cn/gtnhsjgmew.html

[T02] Kotlin：变量
来源：http://hz.jinqigufen.top/gtzjxnqbic.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.smart0.xyz/gtoajwihix.html


<!-- 参考信息 -->