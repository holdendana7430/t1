代发 wailian999

readonly PI=3.14
来源：http://hz.zdqjudy.top/gtbdozhpdn.html

[R04] 位置参数
来源：http://hz.shzxlz.cn/gtcmrkafre.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.pycfn.com/gtiipfvvkh.html

[R05] 参数默认值
来源：http://hz.xziqi.cn/gtvqbrqwde.html

name="${1:-default}"
来源：http://hz.tianlin.xyz/gtivjwuatt.html

[R06] 判断命令是否存在
来源：http://hz.hysaishi.cn/gthulktyzs.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.tianlin.xyz/gtqxqbaajy.html

[R07] if 判断文件
来源：http://hz.wangdashe.top/gtkevmlwcc.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.snrcjt.cn/gtcwwhujmp.html

[R08] 数值比较
来源：http://hz.xingfuxueyuan.xyz/gtmernqswd.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.shuidangran.top/gtvlmertdl.html

[R09] 字符串比较
来源：http://hz.cqqwz.cn/gtnjvhvowl.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.redwolf501.top/gtgvdhelnb.html

[R10] 正则匹配
来源：http://hz.xuetiantiany.cn/gtvrrtsdct.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.aibaodan.cn/gtgigqcesz.html

[R11] case 多分支
来源：http://hz.zhongyouzk.top/gtzcsqxwbs.html

case "$1" in
来源：http://hz.zhijiandao.cn/gtgkevqist.html

start) echo "启动" ;;
来源：http://hz.cucudq.cn/gtzmudoggp.html

stop)  echo "停止" ;;
来源：http://hz.yuanzhike.top/gtqinaibsb.html

*)     echo "未知命令" ;;
来源：http://hz.pycfn.com/gtmrxjbgoo.html

esac
来源：http://hz.chenlongwang.top/gtiwqhckcj.html

[R12] for 遍历文件
来源：http://hz.quarkkingdee.top/gthdjyworw.html

for f in *.txt; do echo "$f"; done
来源：http://hz.zdqjudy.top/gtaaqtqypm.html

[R13] for 计数循环
来源：http://hz.tian-w.cn/gtmguwsdhj.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.haohaochexian.top/gtjtzliwpu.html

[R14] C 风格 for
来源：http://hz.zycfv.cn/gtidxgjffl.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.meibo888.top/gtdfulcvss.html

[R15] while 逐行读文件
来源：http://hz.andypj.xyz/gtzrkhfmgb.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.gotoacloud.top/gtzpptcpbo.html

[R16] until 等待条件
来源：http://hz.jianghu66.top/gtcmtsnyen.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.ivvv.top/gtflxxqjsg.html

[R17] 数组定义与取值
来源：http://hz.jianghu66.top/gtiukwisnl.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.guannengcc.top/gtatumbwdn.html

[R18] 遍历数组
来源：http://hz.xinyue.icu/gthplrstyc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.sxryk.cn/gtbilmocdj.html

[R19] 数组长度
来源：http://hz.yueranfly.top/gtvxslfnab.html

echo "${#arr[@]}"
来源：http://hz.daria6918.cn/gtcrrtmvxy.html

[R20] 关联数组（字典）
来源：http://hz.cucudq.cn/gtpxifmevh.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.zycfv.cn/gtgfkcbtbj.html

[R21] 字符串长度
来源：http://hz.sysykeji.top/gtaupbrsol.html

echo "${#s}"
来源：http://hz.jianghu66.top/gtwqfuwrqc.html

[R22] 截取子串
来源：http://hz.ydzc1.top/gtfkxmyqng.html

echo "${s:0:5}"
来源：http://hz.yj20258.top/gtctinzixo.html

[R23] 字符串替换
来源：http://hz.9152youxi.cn/gthfrdrzlr.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.nanxuanxn.top/gtamhgxibs.html

[R24] 大小写转换
来源：http://hz.ppjwa.cn/gtulhupycz.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.meibo888.top/gtivvtueve.html

[R25] 去后缀 / 去前缀
来源：http://hz.zycfv.cn/gtrtvnhcsj.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.zhiwuduotai.top/gtjmjaxuml.html

[R26] 命令替换
来源：http://hz.hongshengwenyu.top/gtwtyreswu.html

now=$(date +%F); echo "$now"
来源：http://hz.jinqigfzy.top/gtseuosnbl.html

[R27] 算术展开
来源：http://hz.yanxiufei.cn/gttebsobly.html

echo $((1 + 2 * 3))
来源：http://hz.pycfn.com/gtrzeirpqx.html

[R28] 浮点运算
来源：http://hz.birdmap.top/gtwpxxnzzd.html

echo "scale=2; 10/3" | bc
来源：http://hz.nanxinkj.top/gtpfdldqol.html

[R29] 定义函数
来源：http://hz.gaohongyu789.top/gtahpeaebm.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.yongpay.top/gtjwubjrhf.html

[R30] 函数返回状态码
来源：http://hz.feifeiyinyue.top/gtcyrpndze.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.zhoulong.xyz/gtrtcryjmj.html

[R31] 局部变量
来源：http://hz.shanyushiyangkeji.top/gttxilyclw.html

f() { local x=1; echo "$x"; }
来源：http://hz.jlsjyb.cn/gtljzuvviq.html

[R32] 参数个数校验
来源：http://hz.xuanzx.com/gtxzifemng.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.shuidangran.top/gtbzcmrxpt.html

[R33] 捕获错误并提示行号
来源：http://hz.zhijiandao.cn/gtruocbohc.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.hnxiangtu.top/gtnirwvwmt.html

[R34] 退出时清理
来源：http://hz.dianchejie.cn/gtjgsthlhs.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.gaohongyu789.top/gttkidacph.html

[R35] 后台执行并等待
来源：http://hz.gogol.net.cn/gtnaymjdoo.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.chenlongwang.top/gtquznbxli.html

[R36] 并发执行多个任务
来源：http://hz.tanke756.top/gtzzwrmxdk.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.kuanghao11.cn/gtgjwaotgb.html

[R37] 把输出赋给变量
来源：http://hz.feifeiyinyue.top/gtbudqflvo.html

files=$(ls -1)
来源：http://hz.zhengqikj.top/gtqlnxyjht.html

[R38] 管道串联
来源：http://hz.xylfe.cn/gtlzudkopt.html

cat a.txt | grep -i error | wc -l
来源：http://hz.quarkkingdee.top/gttntbfyin.html

[R39] 重定向标准输出与错误
来源：http://hz.tanke756.top/gtsklncsju.html

cmd > out.log 2>&1
来源：http://hz.nanxuanxn.top/gtuniorwyn.html

[R40] 追加写日志
来源：http://hz.cheryme.top/gtqgvdkeyx.html

echo "log" >> out.log
来源：http://hz.xinyue.icu/gtnstmrvdj.html

[R41] 丢弃输出
来源：http://hz.mhx1999.top/gtwaijjlsa.html

cmd >/dev/null 2>&1
来源：http://hz.quarkkingdee.top/gtayahlltl.html

[R42] 输入重定向
来源：http://hz.xingfuxueyuan.xyz/gtwkerumec.html

wc -l < a.txt
来源：http://hz.zhiwuduotai.top/gtolbvworf.html

[R43] 按名字查找文件
来源：http://hz.yueranfly.top/gttftbetnr.html

find . -name "*.log" -type f
来源：http://hz.havefunace.top/gtktaqturh.html

[R44] 按修改时间查找
来源：http://hz.hnqzz.top/gtlflsofgd.html

find . -mtime -7 -type f
来源：http://hz.guannengcc.top/gtlnfyvqgb.html

[R45] 批量删除
来源：http://hz.nwbrower.top/gtpfusufbb.html

find . -name "*.tmp" -delete
来源：http://hz.daxiang520.top/gtocdkumpm.html

[R46] 递归替换文件内容
来源：http://hz.hammf.cn/gtcbwfsguj.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.52xcode.cn/gtdmeiehzr.html

[R47] sed 单行替换
来源：http://hz.yj202588.top/gtrsqgzmlg.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.ywan-chungtsiang.top/gtjsloyikp.html

[R48] awk 取指定列
来源：http://hz.0kj1m.cn/gtkbckxfnk.html

awk '{print $1, $3}' a.txt
来源：http://hz.xziqi.cn/gthrorrekp.html

[R49] awk 带条件
来源：http://hz.andypj.xyz/gtowfrbthq.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.daxiang520.top/gthqnxhmrc.html

[R50] awk 求和
来源：http://hz.shuidangran.top/gtouicginh.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.aizwys.cn/gtqidnsnrm.html

[R51] 排序去重取前几
来源：http://hz.yueranfly.top/gtlanvehaw.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.snrcjt.cn/gtlsycshvv.html

[R52] 统计行数
来源：http://hz.cucudq.cn/gthlsvtpqg.html

wc -l a.txt
来源：http://hz.wangdashe.top/gtpsruberu.html

[R53] 查看文件头与实时尾
来源：http://hz.jyoumei.cn/gtobxujdvq.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.quarkkingdee.top/gtefbjymxw.html

[R54] 比较两个文件
来源：http://hz.yj20258.top/gtjvgdysec.html

diff a.txt b.txt
来源：http://hz.yueranfly.top/gtsxiqkyje.html

[R55] 压缩与解压
来源：http://hz.redwolf501.top/gtmoxzkqlk.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.quarkkingdee.top/gttiyvciye.html

[R56] 远程拷贝
来源：http://hz.haohaochexian.top/gtjucwpnoa.html

scp file user@host:/path/
来源：http://hz.sxryk.cn/gthbssczsp.html

[R57] 远程执行命令
来源：http://hz.9152youxi.cn/gtvvrppftf.html

ssh user@host 'uptime'
来源：http://hz.nwbrower.top/gtudumvvye.html

[R58] 下载文件
来源：http://hz.havefunace.top/gtoaxlhcvg.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.yonumen.top/gtkcfsqieh.html

[R59] 发 POST JSON
来源：http://hz.yuxming.cn/gtordcbmkz.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.smart0.xyz/gtvvntjvni.html

[R60] 只看 HTTP 状态码
来源：http://hz.chenjidiqi.icu/gttqogkgus.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.xziqi.cn/gtqbithcnv.html

[R61] 磁盘占用
来源：http://hz.shanyushiyangtech.top/gtiumkminx.html

df -h;  du -sh *
来源：http://hz.daria6918.cn/gtcrkxvyrn.html

[R62] 找最占空间的文件
来源：http://hz.zhijiandao.cn/gttdgqgncp.html

du -ah . | sort -rh | head -10
来源：http://hz.jinghuilouyu.cn/gtgvninjuh.html

[R63] 内存与进程
来源：http://hz.jinqigfzy.top/gtjvvcmpub.html

free -h;  ps aux | grep nginx
来源：http://hz.jinqigufen.top/gtmgagpteh.html

[R64] 结束进程
来源：http://hz.zdqjudy.top/gtmetjzxzm.html

kill -9 $(pgrep -f app.py)
来源：http://hz.hywenlv.cn/gturbmksld.html

[R65] 查看端口占用
来源：http://hz.jiagoushi.top/gtxdbjpiln.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.chenzaomai.com/gtupbipukh.html

[R66] 定时任务
来源：http://hz.fengsongda.top/gtgzaccpna.html

crontab -e;  crontab -l
来源：http://hz.havefunace.top/gtfyfkuqgl.html

[R67] 生成随机十六进制串
来源：http://hz.wangdashe.top/gtrhhhkuds.html

openssl rand -hex 16
来源：http://hz.xuanzx.com/gtedgdudhf.html

[R68] 计算文件校验值
来源：http://hz.dianchejie.cn/gtzpscgrwm.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.jinqigufen.top/gtwllahxgy.html

[R69] 生成随机密码
来源：http://hz.daxiang520.top/gtuyyzkkpp.html

head -c 16 /dev/urandom | base64
来源：http://hz.smart0.xyz/gtberlsmor.html

[R70] 时间戳与互转
来源：http://hz.jqgufenzy.top/gtbyljvxsm.html

date +%s;  date -d @1700000000
来源：http://hz.quarkkingdee.top/gthxxrlyrn.html

[R71] 日期格式化
来源：http://hz.jinyuanbaomall.cn/gtpcruktsg.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.yangfankeji.com/gtdhzgnoju.html

[R72] 等待端口就绪
来源：http://hz.jlsjyb.cn/gtqezktbvp.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.mhx1999.top/gtkfxzsrrd.html

[R73] 分割大日志
来源：http://hz.andypj.xyz/gtgkzykjao.html

split -l 1000 big.log part_
来源：http://hz.yueranfly.top/gtwdcboded.html

[R74] 批量重命名
来源：http://hz.yj20258888.top/gttlcmgifb.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.fengsongda.top/gtcuvvjxsm.html

[R75] 导出环境变量
来源：http://hz.cqqwz.cn/gtrdllughk.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.chenjidiqi.icu/gtdhtgjpfn.html

[R76] 使用临时文件
来源：http://hz.xuetiantiany.cn/gtbxkfhkua.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.0kj1m.cn/gtipfpakxr.html

[R77] 读取用户输入
来源：http://hz.gogol.net.cn/gtwwxyfhrk.html

read -rp "请输入: " ans
来源：http://hz.shanyushiyangtech.top/gtsxktocqc.html

[R78] 交互式菜单
来源：http://hz.xziqi.cn/gtdbckifjd.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.zhoulong.xyz/gtupvnusec.html

[R79] 解析命令行选项
来源：http://hz.52xcode.cn/gtezewphmk.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.yuanzhike.top/gtuwmalaqb.html

[R80] 查看脚本执行耗时
来源：http://hz.ydzc1.top/gtrpcxeppd.html

time ./run.sh
来源：http://hz.jqgufenzy.top/gtbikuyljh.html

================================================================================
来源：http://hz.zhijiandao.cn/gtrzphtndq.html

S. C / C++ 专题
来源：http://hz.hysaishi.cn/gtqzywhmhf.html

================================================================================
来源：http://hz.jinqigfzy.top/gtrgverjcz.html

[S01] C：Hello World
来源：http://hz.xuanzx.com/gtocuqryog.html

#include <stdio.h>
来源：http://hz.jqgufenzy.top/gtsuhigdwo.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.birdmap.top/gtvoofgfcz.html

[S02] C：变量与格式化输出
来源：http://hz.yangfankeji.com/gtfpkbdpaq.html

int a = 10; printf("%d\n", a);
来源：http://hz.xylfe.cn/gtrxqpyfts.html

[S03] C：读入整数
来源：http://hz.nanxuanxn.top/gtjywxxxou.html

int x; scanf("%d", &x);
来源：http://hz.fzhhl.top/gtghizcnqd.html

[S04] C：字符串复制
来源：http://hz.svipenyu.cn/gtqxrntxvy.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.tianlin.xyz/gtgreyqpip.html

[S05] C：字符串长度
来源：http://hz.tanke756.top/gtqkxczkui.html

strlen(s)
来源：http://hz.daria6918.cn/gtkidkukzn.html

[S06] C：字符串比较
来源：http://hz.ehwqpu.com/gtatgludbn.html

strcmp(a, b) == 0
来源：http://hz.jinqigfzy.top/gtkflnuwii.html

[S07] C：数组遍历求和
来源：http://hz.wangdashe.top/gtywzceswd.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.yuxming.cn/gtqkejivjb.html

[S08] C：动态内存分配与释放
来源：http://hz.xingfuxueyuan.xyz/gtduuwcfef.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.zhijiandao.cn/gtnvxheogf.html

[S09] C：结构体定义与初始化
来源：http://hz.iojbl.cn/gtyclohjbu.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.aibaodan.cn/gtfaftbmii.html

[S10] C：指针与解引用
来源：http://hz.daria6918.cn/gtqsywlqqh.html

int *p = &a;  *p = 5;
来源：http://hz.snrcjt.cn/gtdjastanz.html

[S11] C：逐行读文件
来源：http://hz.hnxiangtu.top/gtmcjdrgda.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.zhoulong.xyz/gtzfullyew.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.feifeiyinyue.top/gtphfbddux.html

fclose(f);
来源：http://hz.jinqigfzy.top/gtltbivxhd.html

[S12] C：写文件
来源：http://hz.aibaodan.cn/gtahnnjcbu.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.jianghu66.top/gtalhljwvv.html

[S13] C：宏定义
来源：http://hz.sufxvd.cn/gtdzhriynn.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.tianlin.xyz/gttebxcvhp.html

[S14] C：枚举
来源：http://hz.hfpthk.cn/gthzzmkqpb.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.cucudq.cn/gticbmebwc.html

[S15] C：类型转换
来源：http://hz.gaohongyu789.top/gtlzhpghcn.html

(double) a / b
来源：http://hz.dianchejie.cn/gtthhivkbs.html

[S16] C：位操作置位
来源：http://hz.sufxvd.cn/gtcsiyfpjv.html

x |= (1 << 3);
来源：http://hz.chenjidiqi.icu/gtzrjgoqcz.html

[S17] C：安全拼接字符串
来源：http://hz.fzhhl.top/gtzfilgsya.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.smart0.xyz/gtavhsssvv.html

[S18] C：命令行参数
来源：http://hz.52xcode.cn/gtaitskncq.html

int main(int argc, char **argv)
来源：http://hz.yongpay.top/gthfhhhugq.html

[S19] C：快速排序
来源：http://hz.zdqjudy.top/gthvxcaqix.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.chenzaomai.com/gtvwxwddiv.html

[S20] C：二分查找
来源：http://hz.pengpengdd.cyou/gtyzilcjox.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.316326.xyz/gtdtwsmjcl.html

[S21] C：字符类别判断
来源：http://hz.kuanghao11.cn/gtwradlywt.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.ivvv.top/gtkjknuoav.html

[S22] C：字符串转数字
来源：http://hz.nwbrower.top/gthryvqneg.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.jinghuilouyu.cn/gtznpggzxs.html

[S23] C：随机数
来源：http://hz.wangshuangyany.cn/gtvoclxntx.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.chenzaomai.com/gtvkazrpao.html

[S24] C：获取本地时间
来源：http://hz.nwbrower.top/gtchsbdzec.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.yvedp.cn/gtspbblacn.html

[S25] C：内存拷贝
来源：http://hz.chenzaomai.com/gtmisqoxfg.html

memcpy(dst, src, n);
来源：http://hz.xziqi.cn/gtmuyzuzcn.html

[S26] C：内存清零
来源：http://hz.316326.xyz/gthyyjjjkx.html

memset(a, 0, sizeof a);
来源：http://hz.haohaochexian.top/gtfrimacwp.html

[S27] C：定义常量
来源：http://hz.xinyue.icu/gtrnmvjmbg.html

const double PI = 3.14159;
来源：http://hz.zhongyouzk.top/gtikxoktek.html

[S28] C：静态变量
来源：http://hz.zycfv.cn/gtxkbmcbpd.html

static int counter = 0;
来源：http://hz.andypj.xyz/gtzfnsgnig.html

[S29] C：变参函数
来源：http://hz.cqqwz.cn/gtjesvoztc.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.nwbrower.top/gtcxkxbstj.html

[S30] C：头文件保护
来源：http://hz.52xcode.cn/gtegambxii.html

#ifndef X_H
来源：http://hz.ydjk.org.cn/gtslezpimc.html

#define X_H
来源：http://hz.yanxiufei.cn/gtphpfnnzu.html

#endif
来源：http://hz.hfpthk.cn/gtlgjtwolb.html

[S31] C++：Hello World
来源：http://hz.quarkkingdee.top/gtgyqrhegv.html

#include <iostream>
来源：http://hz.havefunace.top/gtkyohwlvn.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.zdqjudy.top/gtbkoyaqap.html

[S32] C++：字符串
来源：http://hz.gogol.net.cn/gtgprioash.html

std::string s = "hi";  s += "!";
来源：http://hz.sxryk.cn/gtidjeybrs.html

[S33] C++：vector 增删
来源：http://hz.tianlin.xyz/gtpfbuzhpu.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.chenlongwang.top/gtoshopynn.html

[S34] C++：遍历 vector
来源：http://hz.ivvv.top/gtagirsinj.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.zhaomingkeji.xyz/gtumrqueeh.html

[S35] C++：map
来源：http://hz.cheryme.top/gteyxvowbp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jinghuilouyu.cn/gtquonjegx.html

[S36] C++：unordered_map
来源：http://hz.zhongyouzk.top/gtchahmrdp.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.kuanghao11.cn/gtzqvqyacw.html

[S37] C++：set
来源：http://hz.daria6918.cn/gtlmduzgyb.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.cashguo.top/gtaozcqyox.html

[S38] C++：排序
来源：http://hz.havefunace.top/gtqvbrwxxr.html

std::sort(v.begin(), v.end());
来源：http://hz.jqgufenzy.top/gtgpuhspxs.html

[S39] C++：自定义比较器排序
来源：http://hz.aizwys.cn/gtcpiefowu.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.chenjidiqi.icu/gtsqzgvmtv.html

[S40] C++：查找元素
来源：http://hz.c1oappe.top/gtyuumupsp.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.ivvv.top/gtrwdqerit.html

[S41] C++：类与构造函数
来源：http://hz.fengsongda.top/gtmdvycufi.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.xziqi.cn/gtkuzzftqv.html

[S42] C++：继承与虚函数
来源：http://hz.cashguo.top/gtqzvrmuhz.html

class B : public Base { public: void f() override {} };
来源：http://hz.yuxming.cn/gtejanebxp.html

[S43] C++：智能指针
来源：http://hz.xinyue.icu/gtylomaotn.html

auto p = std::make_unique<int>(5);
来源：http://hz.dianchejie.cn/gtinllwhtn.html

[S44] C++：引用传参
来源：http://hz.jinghuilouyu.cn/gtgbkfzqkk.html

void inc(int &x) { ++x; }
来源：http://hz.svipenyu.cn/gtllnedjqo.html

[S45] C++：lambda
来源：http://hz.wangdashe.top/gtfpqnuepg.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.aizwys.cn/gttfcbbtow.html

[S46] C++：函数模板
来源：http://hz.nwbrower.top/gthbpxugad.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.yanxiufei.cn/gtkumnsexf.html

[S47] C++：结构化绑定遍历
来源：http://hz.ywan-chungtsiang.top/gtylgwdivs.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.shanyushiyangkeji.top/gtmeztwptm.html

[S48] C++：逐行读文件
来源：http://hz.shuidangran.top/gtlcpeudlw.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.xuanzx.com/gtezkjdctj.html

while (std::getline(in, line)) { }
来源：http://hz.cdnleiting.top/gtaficpupj.html

[S49] C++：写文件
来源：http://hz.yuxming.cn/gtcowwslup.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.mhx1999.top/gtlbygwade.html

[S50] C++：格式化数字
来源：http://hz.xuetiantiany.cn/gtdmqnaxfm.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.jinyuanbaomall.cn/gtkmcgqlgv.html

[S51] C++：显式类型转换
来源：http://hz.ivvv.top/gtbhniiarr.html

static_cast<double>(a) / b
来源：http://hz.guannengcc.top/gtplvzybsn.html

[S52] C++：const 与 noexcept
来源：http://hz.havefunace.top/gtizofkrvm.html

int size() const noexcept { return n_; }
来源：http://hz.aibaodan.cn/gtfzptzgnd.html

[S53] C++：移动语义
来源：http://hz.yanxiufei.cn/gtfqnubobr.html

std::vector<int> w = std::move(v);
来源：http://hz.shanyushiyangtech.top/gtxhvfbvir.html

[S54] C++：异常处理
来源：http://hz.haohaochexian.top/gthicbkebn.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.aibaodan.cn/gtixjrgbwk.html

[S55] C++：结构化绑定
来源：http://hz.cheryme.top/gtlunpadmu.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.bjfxy.top/gtcoqjigzx.html

[S56] C++：optional
来源：http://hz.nanxinkj.top/gttnmcidjf.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.guannengcc.top/gtybppjuat.html

[S57] C++：编译期常量
来源：http://hz.jinghuilouyu.cn/gtukxskifs.html

constexpr int N = 10;
来源：http://hz.jianghu66.top/gtajctsssy.html

[S58] C++：命名空间
来源：http://hz.pycfn.com/gtsacwyivp.html

namespace ns { int f() { return 1; } }
来源：http://hz.haohaochexian.top/gtyllbyeaw.html

[S59] C++：静态断言
来源：http://hz.hfpthk.cn/gtxzzscsib.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.c1oappe.top/gtkmtdsppq.html

[S60] C++：遍历并删除元素
来源：http://hz.jlsjyb.cn/gtbxtqftil.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.zhixingplan.top/gtocldmrol.html

================================================================================
来源：http://hz.9152youxi.cn/gtorruccdh.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.fzhhl.top/gtlwrqbzya.html

================================================================================
来源：http://hz.jqgufenzy.top/gtzyhbfmdl.html

[T01] Kotlin：Hello World
来源：http://hz.jinyuanbaomall.cn/gtwkoafxqh.html

println("Hello")
来源：http://hz.havefunace.top/gtuslyjrrd.html

[T02] Kotlin：变量
来源：http://hz.yj20258.top/gtizdrhggy.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.xuanzx.com/gtvshnrftq.html

[T03] Kotlin：字符串模板
来源：http://hz.cdnleiting.top/gtuqwqyemx.html

"值: $b"
来源：http://hz.yj202588.top/gtccbdkpcm.html

[T04] Kotlin：空安全
来源：http://hz.yuanzhike.top/gtcfeezerv.html

val n: String? = null;  n?.length
来源：http://hz.bjfxy.top/gtrhpderzm.html


<!-- 参考信息 -->