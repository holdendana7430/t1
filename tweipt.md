代发 wailian999

set -euo pipefail
来源：http://hz.gogol.net.cn/gtdambrcjl.html

[R02] 变量赋值与使用
来源：http://hz.shzxlz.cn/gtdlynvifl.html

name="Tom"; echo "$name"
来源：http://hz.52xcode.cn/gtdtkxlhwv.html

[R03] 只读变量
来源：http://hz.haohaochexian.top/gthiyjgknk.html

readonly PI=3.14
来源：http://hz.jinqigfzy.top/gtmrremfzb.html

[R04] 位置参数
来源：http://hz.xingfuxueyuan.xyz/gtposrwbnu.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.haohaochexian.top/gtdkvuphep.html

[R05] 参数默认值
来源：http://hz.yuxming.cn/gtdnrbehhv.html

name="${1:-default}"
来源：http://hz.mhx1999.top/gtegrrtdbn.html

[R06] 判断命令是否存在
来源：http://hz.zhiwuduotai.top/gtfhytlvhs.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.jinqigfzy.top/gttoortcnj.html

[R07] if 判断文件
来源：http://hz.sysykeji.top/gtuavdpecd.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.daria6918.cn/gtnlxpygmb.html

[R08] 数值比较
来源：http://hz.jinyuanbaomall.cn/gtnywncofr.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.ywan-chungtsiang.top/gtcbtpyxtd.html

[R09] 字符串比较
来源：http://hz.nanxinkj.top/gtpnrfswun.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.cdnleiting.top/gtmqlezgmn.html

[R10] 正则匹配
来源：http://hz.guannengcc.top/gtjvkaibgz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.hnqzz.top/gtukeotoow.html

[R11] case 多分支
来源：http://hz.hysaishi.cn/gtyaycxxra.html

case "$1" in
来源：http://hz.pengpengdd.cyou/gtsvtpwjpy.html

start) echo "启动" ;;
来源：http://hz.jinghuilouyu.cn/gtlnwffztr.html

stop)  echo "停止" ;;
来源：http://hz.tianlin.xyz/gtqzvvvfln.html

*)     echo "未知命令" ;;
来源：http://hz.gogol.net.cn/gtqhdyscha.html

esac
来源：http://hz.tanke756.top/gtavtfbuld.html

[R12] for 遍历文件
来源：http://hz.wangdashe.top/gtgtwzwglj.html

for f in *.txt; do echo "$f"; done
来源：http://hz.c1oappe.top/gtyaynwrfd.html

[R13] for 计数循环
来源：http://hz.sxryk.cn/gtavbocobb.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.yangfankeji.com/gteryktrii.html

[R14] C 风格 for
来源：http://hz.zhiwuduotai.top/gtjlekgeav.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.shzxlz.cn/gtykyzxhba.html

[R15] while 逐行读文件
来源：http://hz.cashguo.top/gtnfxnmqxx.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.0kj1m.cn/gtzqboewqj.html

[R16] until 等待条件
来源：http://hz.iojbl.cn/gtzzuzrbao.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.hnqzz.top/gtgefjtfjj.html

[R17] 数组定义与取值
来源：http://hz.9152youxi.cn/gttfrgkugl.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.316326.xyz/gtmpodcpao.html

[R18] 遍历数组
来源：http://hz.zhaomingkeji.xyz/gtwwpospfb.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.xuanzx.com/gtqtqwnjzl.html

[R19] 数组长度
来源：http://hz.yvedp.cn/gtksguvtpo.html

echo "${#arr[@]}"
来源：http://hz.vqdsnc.cn/gtshuyhmew.html

[R20] 关联数组（字典）
来源：http://hz.dashuyun.cn/gtnibrmvdq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.tanke756.top/gtzjgxlmux.html

[R21] 字符串长度
来源：http://hz.xziqi.cn/gtlkebhxkj.html

echo "${#s}"
来源：http://hz.aibaodan.cn/gtskmkzkdb.html

[R22] 截取子串
来源：http://hz.hammf.cn/gtvakopepn.html

echo "${s:0:5}"
来源：http://hz.yvedp.cn/gtufhvohuw.html

[R23] 字符串替换
来源：http://hz.jianghu66.top/gtmgyidryu.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.9152youxi.cn/gtxuvyvarw.html

[R24] 大小写转换
来源：http://hz.fzhhl.top/gtsiauxbwh.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.yanxiufei.cn/gtwhhlulhb.html

[R25] 去后缀 / 去前缀
来源：http://hz.0kj1m.cn/gtqtwiwnsi.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.cucudq.cn/gthadunlaw.html

[R26] 命令替换
来源：http://hz.ivvv.top/gtajupuyib.html

now=$(date +%F); echo "$now"
来源：http://hz.yvedp.cn/gtrdgtnarg.html

[R27] 算术展开
来源：http://hz.hongshengwenyu.top/gtqnsntjwe.html

echo $((1 + 2 * 3))
来源：http://hz.dashuyun.cn/gtoexbpktd.html

[R28] 浮点运算
来源：http://hz.zhoulong.xyz/gtapfjsaaj.html

echo "scale=2; 10/3" | bc
来源：http://hz.shanyushiyangtech.top/gttknnnxom.html

[R29] 定义函数
来源：http://hz.xuanzx.com/gtpmlmpquy.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.zhoulong.xyz/gtwjbjpyec.html

[R30] 函数返回状态码
来源：http://hz.zdqjudy.top/gtyatvhwgk.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.yj20258888.top/gtkmgyxqwa.html

[R31] 局部变量
来源：http://hz.hfpthk.cn/gtqworjmxu.html

f() { local x=1; echo "$x"; }
来源：http://hz.hongshengwenyu.top/gtpysmklxx.html

[R32] 参数个数校验
来源：http://hz.hysaishi.cn/gtwxnjbfqn.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.sweek.top/gtntiujstk.html

[R33] 捕获错误并提示行号
来源：http://hz.gotoacloud.top/gtaowlizsz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.zycfv.cn/gtcuyjkuwp.html

[R34] 退出时清理
来源：http://hz.yj20258.top/gtbjsstzhp.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.shanyushiyangtech.top/gtdqzrpufj.html

[R35] 后台执行并等待
来源：http://hz.0kj1m.cn/gtxrpsnxbq.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.52xcode.cn/gtwxxjonzd.html

[R36] 并发执行多个任务
来源：http://hz.kuanghao11.cn/gtfioaijko.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.shanyushiyangtech.top/gtlhsqrgma.html

[R37] 把输出赋给变量
来源：http://hz.meibo888.top/gtfintsfbg.html

files=$(ls -1)
来源：http://hz.havefunace.top/gtpipjuvqa.html

[R38] 管道串联
来源：http://hz.yj20258888.top/gtpidrgure.html

cat a.txt | grep -i error | wc -l
来源：http://hz.meibo888.top/gtdftganvx.html

[R39] 重定向标准输出与错误
来源：http://hz.ydzc1.top/gtphprpzjg.html

cmd > out.log 2>&1
来源：http://hz.zhixingplan.top/gtjbwskllj.html

[R40] 追加写日志
来源：http://hz.guannengcc.top/gtkfrrxlrq.html

echo "log" >> out.log
来源：http://hz.jinqigufen.top/gtgexypzju.html

[R41] 丢弃输出
来源：http://hz.yongpay.top/gtrxsxiizu.html

cmd >/dev/null 2>&1
来源：http://hz.xuetiantiany.cn/gtuaskhzpo.html

[R42] 输入重定向
来源：http://hz.cheryme.top/gtjnbxpagi.html

wc -l < a.txt
来源：http://hz.nwbrower.top/gtfudzxpne.html

[R43] 按名字查找文件
来源：http://hz.jinqigufen.top/gtkrqkglsi.html

find . -name "*.log" -type f
来源：http://hz.xziqi.cn/gtvmccljjx.html

[R44] 按修改时间查找
来源：http://hz.shanyushiyangkeji.top/gtdubntitc.html

find . -mtime -7 -type f
来源：http://hz.zhongyouzk.top/gtiqomqdcz.html

[R45] 批量删除
来源：http://hz.kuanghao11.cn/gtnlofzddc.html

find . -name "*.tmp" -delete
来源：http://hz.xuetiantiany.cn/gtyzifqblu.html

[R46] 递归替换文件内容
来源：http://hz.jinghuilouyu.cn/gtpwwzukac.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.pengpengdd.cyou/gtwwkgrlzh.html

[R47] sed 单行替换
来源：http://hz.cqqwz.cn/gtxomqvxjl.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.hysaishi.cn/gtsskxdpnu.html

[R48] awk 取指定列
来源：http://hz.bjfxy.top/gtklgcntmi.html

awk '{print $1, $3}' a.txt
来源：http://hz.sufxvd.cn/gtljhqmqly.html

[R49] awk 带条件
来源：http://hz.zhoulong.xyz/gtwjvralnr.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.smart0.xyz/gtekqggmch.html

[R50] awk 求和
来源：http://hz.hnxiangtu.top/gtukhpfcfw.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.chenzaomai.com/gtcojdhdit.html

[R51] 排序去重取前几
来源：http://hz.ywan-chungtsiang.top/gtkqnlqivo.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.jqgfzy.top/gtekqohcml.html

[R52] 统计行数
来源：http://hz.daxiang520.top/gtetkwekoc.html

wc -l a.txt
来源：http://hz.yj202588.top/gtnncnuqbg.html

[R53] 查看文件头与实时尾
来源：http://hz.fzhhl.top/gtthywhbpb.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.sysykeji.top/gtepokroqk.html

[R54] 比较两个文件
来源：http://hz.yanxiufei.cn/gtwqqcrwqs.html

diff a.txt b.txt
来源：http://hz.gotoacloud.top/gtipdrklsy.html

[R55] 压缩与解压
来源：http://hz.gaohongyu789.top/gtsdrgrsbl.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.yvedp.cn/gtzhogtyel.html

[R56] 远程拷贝
来源：http://hz.yvedp.cn/gtnlnmtlpm.html

scp file user@host:/path/
来源：http://hz.zhixingplan.top/gtchactuef.html

[R57] 远程执行命令
来源：http://hz.wangdashe.top/gtykjxobrp.html

ssh user@host 'uptime'
来源：http://hz.shangyingyoupin.top/gtzfxybfag.html

[R58] 下载文件
来源：http://hz.fzhhl.top/gtlrngxdgg.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.zhiwuduotai.top/gtmkfhllut.html

[R59] 发 POST JSON
来源：http://hz.shanyushiyangkeji.top/gtlokojggr.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.cashguo.top/gtcchwqeca.html

[R60] 只看 HTTP 状态码
来源：http://hz.daria6918.cn/gtpfduvvpm.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.smart0.xyz/gtmxqwqxhs.html

[R61] 磁盘占用
来源：http://hz.andypj.xyz/gtbwdfeiak.html

df -h;  du -sh *
来源：http://hz.zdqjudy.top/gtwulcemyg.html

[R62] 找最占空间的文件
来源：http://hz.zhiwuduotai.top/gtcmjpecyj.html

du -ah . | sort -rh | head -10
来源：http://hz.birdmap.top/gtcnjmeunb.html

[R63] 内存与进程
来源：http://hz.tanke756.top/gtncejpvhd.html

free -h;  ps aux | grep nginx
来源：http://hz.jqgfzy.top/gtxfrigbuf.html

[R64] 结束进程
来源：http://hz.guowangkeji.top/gtkucrrfuv.html

kill -9 $(pgrep -f app.py)
来源：http://hz.jiagoushi.top/gtxkmmaeyr.html

[R65] 查看端口占用
来源：http://hz.havefunace.top/gtrbpwqstj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.kuanghao11.cn/gthlxksxqb.html

[R66] 定时任务
来源：http://hz.chenzaomai.com/gtuwgzhwko.html

crontab -e;  crontab -l
来源：http://hz.ydzc1.top/gtgqcgglbd.html

[R67] 生成随机十六进制串
来源：http://hz.zhaomingkeji.xyz/gtrkbalsea.html

openssl rand -hex 16
来源：http://hz.hongshengwenyu.top/gtzewucmll.html

[R68] 计算文件校验值
来源：http://hz.chenjidiqi.icu/gtmscrmgns.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.guannengcc.top/gtrjbcwglq.html

[R69] 生成随机密码
来源：http://hz.shuidangran.top/gtgcpbvdfd.html

head -c 16 /dev/urandom | base64
来源：http://hz.guowangkeji.top/gtdpigxjnq.html

[R70] 时间戳与互转
来源：http://hz.guannengcc.top/gtwzyrdmrc.html

date +%s;  date -d @1700000000
来源：http://hz.gogol.net.cn/gtdtuekjxe.html

[R71] 日期格式化
来源：http://hz.smart0.xyz/gtjoeoajvb.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.redwolf501.top/gttqylojmt.html

[R72] 等待端口就绪
来源：http://hz.hysaishi.cn/gtynjrelep.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.dashuyun.cn/gtsbsrpucg.html

[R73] 分割大日志
来源：http://hz.zhoulong.xyz/gthubszmrr.html

split -l 1000 big.log part_
来源：http://hz.zhoulong.xyz/gtfwyauqke.html

[R74] 批量重命名
来源：http://hz.zdqjudy.top/gtajkaotlt.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.meibo888.top/gtwfvcqfrm.html

[R75] 导出环境变量
来源：http://hz.chenzaomai.com/gtszbbdwmz.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.jiagoushi.top/gtmgbpyyej.html

[R76] 使用临时文件
来源：http://hz.yj20258.top/gtwvmihugm.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.jianghu66.top/gtivvvjcok.html

[R77] 读取用户输入
来源：http://hz.cheryme.top/gtdsobrlig.html

read -rp "请输入: " ans
来源：http://hz.hammf.cn/gtktjkjagu.html

[R78] 交互式菜单
来源：http://hz.meibo888.top/gtadbdrswl.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.smart0.xyz/gtxdlczopw.html

[R79] 解析命令行选项
来源：http://hz.mhx1999.top/gtteeqysac.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.xuetiantiany.cn/gtfdenbawp.html

[R80] 查看脚本执行耗时
来源：http://hz.feifeiyinyue.top/gtfobdwrww.html

time ./run.sh
来源：http://hz.c1oappe.top/gtmlptgfck.html

================================================================================
来源：http://hz.xylfe.cn/gtbjijgvxi.html

S. C / C++ 专题
来源：http://hz.zhiwuduotai.top/gtzcysamvc.html

================================================================================
来源：http://hz.jinqigfzy.top/gtgxjwptub.html

[S01] C：Hello World
来源：http://hz.ywan-chungtsiang.top/gtfbhzeaaz.html

#include <stdio.h>
来源：http://hz.jyoumei.cn/gtwqtfxqpg.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.kuanghao11.cn/gthdgsrmvn.html

[S02] C：变量与格式化输出
来源：http://hz.dianchejie.cn/gtgetcydry.html

int a = 10; printf("%d\n", a);
来源：http://hz.cashguo.top/gtnaqxgrva.html

[S03] C：读入整数
来源：http://hz.guannengcc.top/gtcjfylusn.html

int x; scanf("%d", &x);
来源：http://hz.havefunace.top/gtfmhyvaze.html

[S04] C：字符串复制
来源：http://hz.pengpengdd.cyou/gtlgxzegwm.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.shanyushiyangtech.top/gtfzwznami.html

[S05] C：字符串长度
来源：http://hz.pengpengdd.cyou/gtjpakvsay.html

strlen(s)
来源：http://hz.havefunace.top/gtxvymboxq.html

[S06] C：字符串比较
来源：http://hz.chenzaomai.com/gtckyjjzut.html

strcmp(a, b) == 0
来源：http://hz.yuxming.cn/gtoylvczgn.html

[S07] C：数组遍历求和
来源：http://hz.iojbl.cn/gtocsoffda.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.dashuyun.cn/gtytrqewnz.html

[S08] C：动态内存分配与释放
来源：http://hz.jinyuanbaomall.cn/gtfzxweeyg.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.ydzc1.top/gtxawzppew.html

[S09] C：结构体定义与初始化
来源：http://hz.birdmap.top/gtlpfplnqu.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.yvedp.cn/gtcprkuigw.html

[S10] C：指针与解引用
来源：http://hz.xziqi.cn/gtdhwisryq.html

int *p = &a;  *p = 5;
来源：http://hz.yuanzhike.top/gttmkmjipp.html

[S11] C：逐行读文件
来源：http://hz.ivvv.top/gtcatmsnen.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.dianchejie.cn/gticjxnccy.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.sysykeji.top/gtfxknqipr.html

fclose(f);
来源：http://hz.ybcxt.top/gtkzaagnrp.html

[S12] C：写文件
来源：http://hz.hfpthk.cn/gtfkzjxeqh.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.aibaodan.cn/gtveyztfbb.html

[S13] C：宏定义
来源：http://hz.sufxvd.cn/gtoaxfdgev.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.aibaodan.cn/gttothiyax.html

[S14] C：枚举
来源：http://hz.ydzc1.top/gttmsgszpv.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.yanxiufei.cn/gtqdouvrmf.html

[S15] C：类型转换
来源：http://hz.guannengcc.top/gtyootxevl.html

(double) a / b
来源：http://hz.vqdsnc.cn/gtpwuhypvw.html

[S16] C：位操作置位
来源：http://hz.c1oappe.top/gtshzkewcp.html

x |= (1 << 3);
来源：http://hz.dashuyun.cn/gtncnjydyq.html

[S17] C：安全拼接字符串
来源：http://hz.hnxiangtu.top/gtdyrmhbak.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.xylfe.cn/gtbvchdzmk.html

[S18] C：命令行参数
来源：http://hz.yanxiufei.cn/gtiesskgjx.html

int main(int argc, char **argv)
来源：http://hz.sxryk.cn/gthkbgssjk.html

[S19] C：快速排序
来源：http://hz.jiagoushi.top/gtioyyxrej.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.zycfv.cn/gtwipgmzel.html

[S20] C：二分查找
来源：http://hz.cqqwz.cn/gtcnjzrezb.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.kuanghao11.cn/gtoobwmrav.html

[S21] C：字符类别判断
来源：http://hz.xuetiantiany.cn/gtejrtjffl.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.jiagoushi.top/gtdfdfpldm.html

[S22] C：字符串转数字
来源：http://hz.pengpengdd.cyou/gtcrjrhxsa.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.sufxvd.cn/gtncquvtig.html

[S23] C：随机数
来源：http://hz.meibo888.top/gtyhigwath.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.ywan-chungtsiang.top/gtwmfaagdx.html

[S24] C：获取本地时间
来源：http://hz.gotoacloud.top/gthxyvlewy.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.jqgufenzy.top/gtpmrxdeqf.html

[S25] C：内存拷贝
来源：http://hz.yuxming.cn/gtcbxxafsv.html

memcpy(dst, src, n);
来源：http://hz.xinyue.icu/gtuqkbwdfo.html

[S26] C：内存清零
来源：http://hz.zhongyouzk.top/gtrydcczjt.html

memset(a, 0, sizeof a);
来源：http://hz.wangdashe.top/gtarwycwbw.html

[S27] C：定义常量
来源：http://hz.pycfn.com/gtcfaywgzy.html

const double PI = 3.14159;
来源：http://hz.zhoulong.xyz/gtbpacrobm.html

[S28] C：静态变量
来源：http://hz.hammf.cn/gtsierbhra.html

static int counter = 0;
来源：http://hz.hongshengwenyu.top/gtpsgmuunv.html

[S29] C：变参函数
来源：http://hz.zhoulong.xyz/gtyikdipit.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.smart0.xyz/gtoyborvvb.html

[S30] C：头文件保护
来源：http://hz.zhengqikj.top/gtsvmtwlre.html

#ifndef X_H
来源：http://hz.cheryme.top/gttakmjtmv.html

#define X_H
来源：http://hz.ybcxt.top/gtopzoizeo.html

#endif
来源：http://hz.yj20258888.top/gtjktebddk.html

[S31] C++：Hello World
来源：http://hz.yj20258888.top/gtnsxqfryh.html

#include <iostream>
来源：http://hz.aizwys.cn/gttshudxic.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.316326.xyz/gtjmkpojdi.html

[S32] C++：字符串
来源：http://hz.cqqwz.cn/gtfhskyhes.html

std::string s = "hi";  s += "!";
来源：http://hz.ivvv.top/gtyjpbhfap.html

[S33] C++：vector 增删
来源：http://hz.xuanzx.com/gtnhnrqtrv.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.ehwqpu.com/gtkxifmfuu.html

[S34] C++：遍历 vector
来源：http://hz.c1oappe.top/gtfoqqimxp.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.zdqjudy.top/gtkiusecao.html

[S35] C++：map
来源：http://hz.meibo888.top/gtrdfneovw.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zhiwuduotai.top/gtwhbvyhsk.html

[S36] C++：unordered_map
来源：http://hz.hnqzz.top/gtgmwomibp.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jlsjyb.cn/gtxtrytxla.html

[S37] C++：set
来源：http://hz.ywan-chungtsiang.top/gtuhmfsasb.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.iojbl.cn/gtyrlomlvk.html

[S38] C++：排序
来源：http://hz.yanxiufei.cn/gtbxkyxlpy.html

std::sort(v.begin(), v.end());
来源：http://hz.gogol.net.cn/gtxttcaaof.html

[S39] C++：自定义比较器排序
来源：http://hz.cheryme.top/gtclrbztjn.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.yj20258888.top/gtojacxruk.html

[S40] C++：查找元素
来源：http://hz.shanyushiyangtech.top/gthyqzktlw.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.yueranfly.top/gterhxfsxj.html

[S41] C++：类与构造函数
来源：http://hz.dianchejie.cn/gtxojldgqo.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.aizwys.cn/gtikvoyqvx.html

[S42] C++：继承与虚函数
来源：http://hz.snrcjt.cn/gtlmwdgofw.html

class B : public Base { public: void f() override {} };
来源：http://hz.shanyushiyangtech.top/gtsxkucvsw.html

[S43] C++：智能指针
来源：http://hz.zhengqikj.top/gtwrfvxbjw.html

auto p = std::make_unique<int>(5);
来源：http://hz.xinyue.icu/gtdbtoqcyu.html

[S44] C++：引用传参
来源：http://hz.guowangkeji.top/gtktjihahu.html

void inc(int &x) { ++x; }
来源：http://hz.316326.xyz/gtchsludra.html

[S45] C++：lambda
来源：http://hz.shanyushiyangtech.top/gtwmknfwej.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.wangshuangyany.cn/gtbenmvcyy.html

[S46] C++：函数模板
来源：http://hz.hongshengwenyu.top/gtjiogygvh.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.shangyingyoupin.top/gtbeorfgsf.html

[S47] C++：结构化绑定遍历
来源：http://hz.pycfn.com/gtykurnlmb.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.zhixingplan.top/gtsotltrpx.html

[S48] C++：逐行读文件
来源：http://hz.gotoacloud.top/gtmvaccufc.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.jqgfzy.top/gtqslxoolo.html

while (std::getline(in, line)) { }
来源：http://hz.zhiwuduotai.top/gtghmymtnd.html

[S49] C++：写文件
来源：http://hz.cheryme.top/gttzkryutk.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.sufxvd.cn/gtpfgbtluo.html

[S50] C++：格式化数字
来源：http://hz.iojbl.cn/gtfxglqpbo.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.hnqzz.top/gtrfhqfkqq.html

[S51] C++：显式类型转换
来源：http://hz.xinyue.icu/gtphymdkro.html

static_cast<double>(a) / b
来源：http://hz.shanyushiyangtech.top/gtarnskfuz.html

[S52] C++：const 与 noexcept
来源：http://hz.jyoumei.cn/gtvhywzoxx.html

int size() const noexcept { return n_; }
来源：http://hz.ywan-chungtsiang.top/gtgyaaniwq.html

[S53] C++：移动语义
来源：http://hz.meibo888.top/gtzqrfozbj.html

std::vector<int> w = std::move(v);
来源：http://hz.andypj.xyz/gteorenaib.html

[S54] C++：异常处理
来源：http://hz.guannengcc.top/gtavmymjjx.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.sysykeji.top/gtasbmsvcy.html

[S55] C++：结构化绑定
来源：http://hz.zhongyouzk.top/gtpzwmbaod.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.ydjk.org.cn/gtnwkqxzhx.html

[S56] C++：optional
来源：http://hz.hnqzz.top/gtpnuwjqgk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.cashguo.top/gtjmxpqzgn.html

[S57] C++：编译期常量
来源：http://hz.cdnleiting.top/gtssoxemle.html

constexpr int N = 10;
来源：http://hz.sweek.top/gtotekngrv.html

[S58] C++：命名空间
来源：http://hz.9152youxi.cn/gtukodrhzi.html

namespace ns { int f() { return 1; } }
来源：http://hz.daria6918.cn/gtispjlugl.html

[S59] C++：静态断言
来源：http://hz.ydjk.org.cn/gtqfzcahzh.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.jqgufenzy.top/gtnibotbxp.html

[S60] C++：遍历并删除元素
来源：http://hz.zhaomingkeji.xyz/gtkwnzyaap.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.cheryme.top/gtiglppdau.html

================================================================================
来源：http://hz.52xcode.cn/gtltjanbix.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.feifeiyinyue.top/gtbzrtwpyf.html

================================================================================
来源：http://hz.dianchejie.cn/gthbjyjmeb.html

[T01] Kotlin：Hello World
来源：http://hz.sxryk.cn/gthlaeaqwa.html

println("Hello")
来源：http://hz.shuidangran.top/gtcywuhshv.html

[T02] Kotlin：变量
来源：http://hz.zdqjudy.top/gtqkssvjha.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.cdnleiting.top/gtklabyisw.html


<!-- 参考信息 -->