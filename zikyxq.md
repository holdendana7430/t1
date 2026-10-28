代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.316326.xyz/gtkxhtkyrk.html

[R08] 数值比较
来源：http://hz.shanyushiyangtech.top/gtgmzhkgbw.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.haohaochexian.top/gtehaoklaj.html

[R09] 字符串比较
来源：http://hz.sysykeji.top/gtldzezpos.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.snrcjt.cn/gtqbdhoyca.html

[R10] 正则匹配
来源：http://hz.vqdsnc.cn/gtlyerxrbv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.chenzaomai.com/gtfiqcnrlq.html

[R11] case 多分支
来源：http://hz.vqdsnc.cn/gthzklsjap.html

case "$1" in
来源：http://hz.guannengcc.top/gtptrahzjk.html

start) echo "启动" ;;
来源：http://hz.yuanzhike.top/gtuvgfrkaa.html

stop)  echo "停止" ;;
来源：http://hz.hongshengwenyu.top/gtwlcwwuip.html

*)     echo "未知命令" ;;
来源：http://hz.haohaochexian.top/gtucshmcmq.html

esac
来源：http://hz.ydjk.org.cn/gtutxymhhr.html

[R12] for 遍历文件
来源：http://hz.jqgufenzy.top/gttmspcysi.html

for f in *.txt; do echo "$f"; done
来源：http://hz.havefunace.top/gthihfetvu.html

[R13] for 计数循环
来源：http://hz.yj20258.top/gtorqazxcp.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.xinyue.icu/gtmtyhtkxv.html

[R14] C 风格 for
来源：http://hz.jinyuanbaomall.cn/gtcxoxertl.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.havefunace.top/gtdjajgvbh.html

[R15] while 逐行读文件
来源：http://hz.sysykeji.top/gtyxxadrdo.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.c1oappe.top/gtemjqcypx.html

[R16] until 等待条件
来源：http://hz.jinghuilouyu.cn/gtrittdovw.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.bjfxy.top/gttbfzlxcs.html

[R17] 数组定义与取值
来源：http://hz.9152youxi.cn/gtwswlofoy.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.havefunace.top/gtmixkjliv.html

[R18] 遍历数组
来源：http://hz.ivvv.top/gtkaxyycwl.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.xuanzx.com/gtgajqmtuo.html

[R19] 数组长度
来源：http://hz.sweek.top/gtwdsflfbt.html

echo "${#arr[@]}"
来源：http://hz.ivvv.top/gtagzpasdv.html

[R20] 关联数组（字典）
来源：http://hz.zhongyouzk.top/gteqgbkkyb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.bjfxy.top/gtcunpxznk.html

[R21] 字符串长度
来源：http://hz.zycfv.cn/gtbquidagx.html

echo "${#s}"
来源：http://hz.zhengqikj.top/gtbawpween.html

[R22] 截取子串
来源：http://hz.aibaodan.cn/gtvbjzjazr.html

echo "${s:0:5}"
来源：http://hz.tanke756.top/gtdxceqtio.html

[R23] 字符串替换
来源：http://hz.yvedp.cn/gtdbhcwadg.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.yj20258.top/gtymqykwrs.html

[R24] 大小写转换
来源：http://hz.cqqwz.cn/gtqwbgnvlo.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.c1oappe.top/gthgjexshf.html

[R25] 去后缀 / 去前缀
来源：http://hz.52xcode.cn/gtpugtlehg.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.hammf.cn/gtxpgbtijp.html

[R26] 命令替换
来源：http://hz.zhixingplan.top/gtfscesjvf.html

now=$(date +%F); echo "$now"
来源：http://hz.snrcjt.cn/gtrokgqxbq.html

[R27] 算术展开
来源：http://hz.zhengqikj.top/gtztmyawcr.html

echo $((1 + 2 * 3))
来源：http://hz.quarkkingdee.top/gtoemaosao.html

[R28] 浮点运算
来源：http://hz.c1oappe.top/gtprsdmyyr.html

echo "scale=2; 10/3" | bc
来源：http://hz.gzhubu.top/gtsejosjyq.html

[R29] 定义函数
来源：http://hz.zhoulong.xyz/gthezfkeef.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.tanke756.top/gtslhkdygb.html

[R30] 函数返回状态码
来源：http://hz.hnqzz.top/gtxokopckb.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.zhixingplan.top/gtpfepnzrk.html

[R31] 局部变量
来源：http://hz.hfpthk.cn/gtbzqvpgjd.html

f() { local x=1; echo "$x"; }
来源：http://hz.yuanzhike.top/gtcjneihhp.html

[R32] 参数个数校验
来源：http://hz.xingfuxueyuan.xyz/gtkrvwwwps.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.yonumen.top/gtefngbvan.html

[R33] 捕获错误并提示行号
来源：http://hz.kuanghao11.cn/gtaburgdjl.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.kuanghao11.cn/gtiwcdhnwz.html

[R34] 退出时清理
来源：http://hz.feifeiyinyue.top/gtjmylfcoq.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.zhijiandao.cn/gtgalppgja.html

[R35] 后台执行并等待
来源：http://hz.hfpthk.cn/gtlbbgotrf.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.yj20258.top/gtrarljbfu.html

[R36] 并发执行多个任务
来源：http://hz.yongpay.top/gtoznphbfd.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.nanxinkj.top/gtzmcehnln.html

[R37] 把输出赋给变量
来源：http://hz.cheryme.top/gtbozcrpnm.html

files=$(ls -1)
来源：http://hz.birdmap.top/gteogzqjxq.html

[R38] 管道串联
来源：http://hz.zdqjudy.top/gtngpnpkbj.html

cat a.txt | grep -i error | wc -l
来源：http://hz.guannengcc.top/gtmlyxogla.html

[R39] 重定向标准输出与错误
来源：http://hz.feifeiyinyue.top/gthnanqmsh.html

cmd > out.log 2>&1
来源：http://hz.andypj.xyz/gtgogixamc.html

[R40] 追加写日志
来源：http://hz.jiagoushi.top/gttnukbwxp.html

echo "log" >> out.log
来源：http://hz.sysykeji.top/gtckllobis.html

[R41] 丢弃输出
来源：http://hz.jlsjyb.cn/gtzuycnffi.html

cmd >/dev/null 2>&1
来源：http://hz.nwbrower.top/gtkqrpznaf.html

[R42] 输入重定向
来源：http://hz.bjfxy.top/gtjvqqhigq.html

wc -l < a.txt
来源：http://hz.cdnleiting.top/gtkiuaqvcg.html

[R43] 按名字查找文件
来源：http://hz.iojbl.cn/gtjpkgukqp.html

find . -name "*.log" -type f
来源：http://hz.yueranfly.top/gtoxnqiwdb.html

[R44] 按修改时间查找
来源：http://hz.xuanzx.com/gtrlthhoim.html

find . -mtime -7 -type f
来源：http://hz.hfpthk.cn/gtlvytobtu.html

[R45] 批量删除
来源：http://hz.yonumen.top/gtzbidgkti.html

find . -name "*.tmp" -delete
来源：http://hz.hnqzz.top/gtqgnygjka.html

[R46] 递归替换文件内容
来源：http://hz.zycfv.cn/gtpfyhtjpy.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.snrcjt.cn/gtubepckxg.html

[R47] sed 单行替换
来源：http://hz.meibo888.top/gtbqeyzyuk.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.sysykeji.top/gtkxtfqlke.html

[R48] awk 取指定列
来源：http://hz.9152youxi.cn/gtglwlpwno.html

awk '{print $1, $3}' a.txt
来源：http://hz.bjfxy.top/gtanrkmtps.html

[R49] awk 带条件
来源：http://hz.guannengcc.top/gtxshokdfm.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.ivvv.top/gtywyocpnn.html

[R50] awk 求和
来源：http://hz.yuanzhike.top/gtjjnvhgto.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.redwolf501.top/gtuzzvubov.html

[R51] 排序去重取前几
来源：http://hz.andypj.xyz/gtnmsnylbm.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.cashguo.top/gtrwmyfvck.html

[R52] 统计行数
来源：http://hz.shangyingyoupin.top/gtqsxxkrsh.html

wc -l a.txt
来源：http://hz.pengpengdd.cyou/gtbazntgjh.html

[R53] 查看文件头与实时尾
来源：http://hz.redwolf501.top/gtjchhkwte.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.ivvv.top/gtczvhdvfz.html

[R54] 比较两个文件
来源：http://hz.yuxming.cn/gtmlyrzezy.html

diff a.txt b.txt
来源：http://hz.yonumen.top/gtaeusqdbh.html

[R55] 压缩与解压
来源：http://hz.yuxming.cn/gtdjpnjyst.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.ydzc1.top/gtgvegswnw.html

[R56] 远程拷贝
来源：http://hz.yvedp.cn/gtajzhglrl.html

scp file user@host:/path/
来源：http://hz.redwolf501.top/gtuowrwphw.html

[R57] 远程执行命令
来源：http://hz.dianchejie.cn/gtknjdpzaa.html

ssh user@host 'uptime'
来源：http://hz.daxiang520.top/gtiofxfltl.html

[R58] 下载文件
来源：http://hz.jyoumei.cn/gtujmjnedx.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.yj202588.top/gtmqjzmjbj.html

[R59] 发 POST JSON
来源：http://hz.cdnleiting.top/gtsabaqtzq.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.shuidangran.top/gtcqdskjed.html

[R60] 只看 HTTP 状态码
来源：http://hz.quarkkingdee.top/gtzhptkkxd.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.cdnleiting.top/gtwhiezijh.html

[R61] 磁盘占用
来源：http://hz.quarkkingdee.top/gtstgfvuzz.html

df -h;  du -sh *
来源：http://hz.cqqwz.cn/gtppgchhto.html

[R62] 找最占空间的文件
来源：http://hz.shangyingyoupin.top/gtvgnuogph.html

du -ah . | sort -rh | head -10
来源：http://hz.ivvv.top/gtjjjgaslh.html

[R63] 内存与进程
来源：http://hz.hywenlv.cn/gtysrqxkxe.html

free -h;  ps aux | grep nginx
来源：http://hz.tian-w.cn/gtailhbgzb.html

[R64] 结束进程
来源：http://hz.yj20258.top/gtpfnongyo.html

kill -9 $(pgrep -f app.py)
来源：http://hz.pycfn.com/gtcnkczdme.html

[R65] 查看端口占用
来源：http://hz.birdmap.top/gtvkonlscm.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.shuidangran.top/gthhfumhep.html

[R66] 定时任务
来源：http://hz.jqgfzy.top/gtozobjgug.html

crontab -e;  crontab -l
来源：http://hz.jqgfzy.top/gtwoslpoqi.html

[R67] 生成随机十六进制串
来源：http://hz.ydjk.org.cn/gtggckxtmb.html

openssl rand -hex 16
来源：http://hz.yonumen.top/gtogrckzfj.html

[R68] 计算文件校验值
来源：http://hz.meibo888.top/gtgxicdoiw.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.yvedp.cn/gtciswasxu.html

[R69] 生成随机密码
来源：http://hz.jinyuanbaomall.cn/gttqvxptcp.html

head -c 16 /dev/urandom | base64
来源：http://hz.mhx1999.top/gtwmumbbgz.html

[R70] 时间戳与互转
来源：http://hz.nwbrower.top/gtzqxvfxyn.html

date +%s;  date -d @1700000000
来源：http://hz.yj20258.top/gtxgakshhx.html

[R71] 日期格式化
来源：http://hz.nanxuanxn.top/gtovzmggoc.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.tanke756.top/gtccnljtvf.html

[R72] 等待端口就绪
来源：http://hz.svipenyu.cn/gtmqeikhii.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.cashguo.top/gtwbjxiirn.html

[R73] 分割大日志
来源：http://hz.cdnleiting.top/gtyykcblvo.html

split -l 1000 big.log part_
来源：http://hz.feifeiyinyue.top/gtiyufuojk.html

[R74] 批量重命名
来源：http://hz.yj20258.top/gtcnlmumgj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.sweek.top/gthajtxnfa.html

[R75] 导出环境变量
来源：http://hz.feifeiyinyue.top/gtirhfbrhw.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.yj20258888.top/gtisrqkdhy.html

[R76] 使用临时文件
来源：http://hz.zdqjudy.top/gtcffnwhqc.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.mhx1999.top/gtyretgomg.html

[R77] 读取用户输入
来源：http://hz.guowangkeji.top/gtiquklufj.html

read -rp "请输入: " ans
来源：http://hz.redwolf501.top/gtkyiwnccz.html

[R78] 交互式菜单
来源：http://hz.fengsongda.top/gtlcjtbvtf.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.guowangkeji.top/gtrhrwrvza.html

[R79] 解析命令行选项
来源：http://hz.chenlongwang.top/gthopfhmqu.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.quarkkingdee.top/gtkplhcvas.html

[R80] 查看脚本执行耗时
来源：http://hz.pengpengdd.cyou/gtpewsiegc.html

time ./run.sh
来源：http://hz.xuetiantiany.cn/gtlyyklxpz.html

================================================================================
来源：http://hz.9152youxi.cn/gtmohijwxw.html

S. C / C++ 专题
来源：http://hz.chenjidiqi.icu/gtyeujexsr.html

================================================================================
来源：http://hz.shuidangran.top/gttbqlyppa.html

[S01] C：Hello World
来源：http://hz.xuanzx.com/gtslzhqcer.html

#include <stdio.h>
来源：http://hz.shuidangran.top/gtgjsxihjg.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.52xcode.cn/gtdfgpsxbu.html

[S02] C：变量与格式化输出
来源：http://hz.zhiwuduotai.top/gtihftdrup.html

int a = 10; printf("%d\n", a);
来源：http://hz.iojbl.cn/gttravonmv.html

[S03] C：读入整数
来源：http://hz.fzhhl.top/gtugoxgjhn.html

int x; scanf("%d", &x);
来源：http://hz.xinyue.icu/gtgbeatwqi.html

[S04] C：字符串复制
来源：http://hz.ehwqpu.com/gtqtfwaqws.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.smart0.xyz/gtexpwrquh.html

[S05] C：字符串长度
来源：http://hz.jyoumei.cn/gtsuwburkt.html

strlen(s)
来源：http://hz.guowangkeji.top/gtrzyotgbh.html

[S06] C：字符串比较
来源：http://hz.birdmap.top/gtzdpwvocj.html

strcmp(a, b) == 0
来源：http://hz.yvedp.cn/gtctmgowzi.html

[S07] C：数组遍历求和
来源：http://hz.yueranfly.top/gtrixhefnd.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.haohaochexian.top/gtzckiiwtt.html

[S08] C：动态内存分配与释放
来源：http://hz.ppjwa.cn/gtgdhqvonh.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.jinghuilouyu.cn/gtvjnkjhkx.html

[S09] C：结构体定义与初始化
来源：http://hz.zhoulong.xyz/gtyiiypzup.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.ivvv.top/gtdaqrgfry.html

[S10] C：指针与解引用
来源：http://hz.haohaochexian.top/gtbjhavmtr.html

int *p = &a;  *p = 5;
来源：http://hz.shanyushiyangtech.top/gtzypbzcoc.html

[S11] C：逐行读文件
来源：http://hz.yuxming.cn/gthdxwjlbq.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.haohaochexian.top/gtgqariyke.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.gzhubu.top/gtvgnduhkw.html

fclose(f);
来源：http://hz.cdnleiting.top/gtxxffeiom.html

[S12] C：写文件
来源：http://hz.yj20258.top/gthnyutkhd.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.yonumen.top/gtfsaduyjh.html

[S13] C：宏定义
来源：http://hz.jqgufenzy.top/gtbrhebyyd.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.pycfn.com/gteybobolb.html

[S14] C：枚举
来源：http://hz.daxiang520.top/gthnwwoafn.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.yj202588.top/gtkxcozmct.html

[S15] C：类型转换
来源：http://hz.zhoulong.xyz/gtjaphvzth.html

(double) a / b
来源：http://hz.hammf.cn/gtpfpckmym.html

[S16] C：位操作置位
来源：http://hz.tanke756.top/gtulouvlmo.html

x |= (1 << 3);
来源：http://hz.ywan-chungtsiang.top/gtlrwjtdlp.html

[S17] C：安全拼接字符串
来源：http://hz.0kj1m.cn/gtayeoxjyj.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.hnxiangtu.top/gtlkpbejof.html

[S18] C：命令行参数
来源：http://hz.ppjwa.cn/gtqaacngkq.html

int main(int argc, char **argv)
来源：http://hz.pengpengdd.cyou/gtlwtzdbwy.html

[S19] C：快速排序
来源：http://hz.zhiwuduotai.top/gtpmcjraps.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.chenzaomai.com/gtaaydqnit.html

[S20] C：二分查找
来源：http://hz.yvedp.cn/gtehylopzd.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.ybcxt.top/gtuofmykuf.html

[S21] C：字符类别判断
来源：http://hz.gogol.net.cn/gtqhgcrhqh.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.zhongyouzk.top/gtyzdcprju.html

[S22] C：字符串转数字
来源：http://hz.zhixingplan.top/gtipyypkwe.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.yonumen.top/gtcrqvpinn.html

[S23] C：随机数
来源：http://hz.sufxvd.cn/gtykjoflcf.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.jinyuanbaomall.cn/gtwrnngxef.html

[S24] C：获取本地时间
来源：http://hz.yanxiufei.cn/gtknoihkmm.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.pengpengdd.cyou/gtcljrshyf.html

[S25] C：内存拷贝
来源：http://hz.shangyingyoupin.top/gtdekpshwz.html

memcpy(dst, src, n);
来源：http://hz.jinghuilouyu.cn/gtxioukkdr.html

[S26] C：内存清零
来源：http://hz.vqdsnc.cn/gtroqiwzlq.html

memset(a, 0, sizeof a);
来源：http://hz.tian-w.cn/gtmdfijeuo.html

[S27] C：定义常量
来源：http://hz.hongshengwenyu.top/gtvdhvwghi.html

const double PI = 3.14159;
来源：http://hz.zhongyouzk.top/gtrncflefg.html

[S28] C：静态变量
来源：http://hz.feifeiyinyue.top/gtwutfcvid.html

static int counter = 0;
来源：http://hz.ivvv.top/gtkhvsyvmo.html

[S29] C：变参函数
来源：http://hz.yangfankeji.com/gtvzpymnnc.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.zhaomingkeji.xyz/gtsvtspbpe.html

[S30] C：头文件保护
来源：http://hz.meibo888.top/gtklasvomh.html

#ifndef X_H
来源：http://hz.hnqzz.top/gtcpxkxtpu.html

#define X_H
来源：http://hz.ybcxt.top/gtdsjeqnpw.html

#endif
来源：http://hz.nanxuanxn.top/gtddrwhmyx.html

[S31] C++：Hello World
来源：http://hz.ybcxt.top/gtvyowqjzf.html

#include <iostream>
来源：http://hz.ydzc1.top/gtukoaywfa.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.daria6918.cn/gtuhloapbx.html

[S32] C++：字符串
来源：http://hz.zhengqikj.top/gtjllegihu.html

std::string s = "hi";  s += "!";
来源：http://hz.zycfv.cn/gtogwirttd.html

[S33] C++：vector 增删
来源：http://hz.yvedp.cn/gtcsvivphw.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.shuidangran.top/gtemsyybfm.html

[S34] C++：遍历 vector
来源：http://hz.birdmap.top/gthnrwrszw.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.cucudq.cn/gtkxxwqupt.html

[S35] C++：map
来源：http://hz.guannengcc.top/gtfeiqtxnp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.c1oappe.top/gtycrlzmlm.html

[S36] C++：unordered_map
来源：http://hz.dashuyun.cn/gtkbocginn.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.nanxinkj.top/gtvjmizahp.html

[S37] C++：set
来源：http://hz.ivvv.top/gtiuzypurj.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.zhaomingkeji.xyz/gtmhdermyo.html

[S38] C++：排序
来源：http://hz.kuanghao11.cn/gtxdlxzmhs.html

std::sort(v.begin(), v.end());
来源：http://hz.daxiang520.top/gtwkacsdxv.html

[S39] C++：自定义比较器排序
来源：http://hz.hywenlv.cn/gtdkkvwbnl.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.yuanzhike.top/gtnlavwuhx.html

[S40] C++：查找元素
来源：http://hz.kuanghao11.cn/gtefcjcmhi.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.hnqzz.top/gtqmcpfjsy.html

[S41] C++：类与构造函数
来源：http://hz.zhiwuduotai.top/gtifvfvbnn.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.zhongyouzk.top/gtfyfejzpy.html

[S42] C++：继承与虚函数
来源：http://hz.xingfuxueyuan.xyz/gtabxugbzg.html

class B : public Base { public: void f() override {} };
来源：http://hz.xingfuxueyuan.xyz/gtkggdjart.html

[S43] C++：智能指针
来源：http://hz.ydzc1.top/gtpbqpaolt.html

auto p = std::make_unique<int>(5);
来源：http://hz.dashuyun.cn/gtuwjxxiwc.html

[S44] C++：引用传参
来源：http://hz.hnxiangtu.top/gtwjtycldi.html

void inc(int &x) { ++x; }
来源：http://hz.ppjwa.cn/gtzzzdtyou.html

[S45] C++：lambda
来源：http://hz.jqgufenzy.top/gtcflceaxw.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.aizwys.cn/gtpkeiatqu.html

[S46] C++：函数模板
来源：http://hz.jqgfzy.top/gtzihmbhdh.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.316326.xyz/gtynondsgl.html

[S47] C++：结构化绑定遍历
来源：http://hz.jqgfzy.top/gtjflektmj.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.zhiwuduotai.top/gtokwbtugx.html

[S48] C++：逐行读文件
来源：http://hz.jqgfzy.top/gtzbzplrpu.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.yonumen.top/gtiyhlhbah.html

while (std::getline(in, line)) { }
来源：http://hz.yj202588.top/gtzecjcskg.html

[S49] C++：写文件
来源：http://hz.kuanghao11.cn/gtdtgfvfcg.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.yongpay.top/gtbowivuuu.html

[S50] C++：格式化数字
来源：http://hz.yueranfly.top/gtofetmvvk.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.ehwqpu.com/gtysugzbqf.html

[S51] C++：显式类型转换
来源：http://hz.hywenlv.cn/gtorrnqywl.html

static_cast<double>(a) / b
来源：http://hz.yonumen.top/gtugugokgd.html

[S52] C++：const 与 noexcept
来源：http://hz.snrcjt.cn/gtbzcstxgr.html

int size() const noexcept { return n_; }
来源：http://hz.sysykeji.top/gtcscfakne.html

[S53] C++：移动语义
来源：http://hz.shzxlz.cn/gtnsvigatx.html

std::vector<int> w = std::move(v);
来源：http://hz.yuxming.cn/gtoehupftc.html

[S54] C++：异常处理
来源：http://hz.zhongyouzk.top/gtwqbljppi.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.yj20258.top/gtmmweasyp.html

[S55] C++：结构化绑定
来源：http://hz.jyoumei.cn/gtlnvdqqqi.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.svipenyu.cn/gtpiepcvfq.html

[S56] C++：optional
来源：http://hz.shanyushiyangkeji.top/gtvpmmexis.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.ydzc1.top/gtienqsrzr.html

[S57] C++：编译期常量
来源：http://hz.nwbrower.top/gtlbxqxdvj.html

constexpr int N = 10;
来源：http://hz.shuidangran.top/gtwitvalwm.html

[S58] C++：命名空间
来源：http://hz.xziqi.cn/gttucdiosz.html

namespace ns { int f() { return 1; } }
来源：http://hz.aizwys.cn/gtbteeyggj.html

[S59] C++：静态断言
来源：http://hz.feifeiyinyue.top/gtkcsfrvff.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.shanyushiyangtech.top/gtbrxqirgp.html

[S60] C++：遍历并删除元素
来源：http://hz.chenjidiqi.icu/gtshkjrhic.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.tian-w.cn/gtnnwpbwbt.html

================================================================================
来源：http://hz.jiagoushi.top/gtsivtdkud.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.fzhhl.top/gtscrvwcsl.html

================================================================================
来源：http://hz.sxryk.cn/gtebkmpwth.html

[T01] Kotlin：Hello World
来源：http://hz.ehwqpu.com/gtgjbjhyaj.html

println("Hello")
来源：http://hz.52xcode.cn/gtohsujkdd.html

[T02] Kotlin：变量
来源：http://hz.jinghuilouyu.cn/gtqvcbizmq.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.cdnleiting.top/gtwqaouhql.html

[T03] Kotlin：字符串模板
来源：http://hz.hnqzz.top/gtrxnlcbox.html

"值: $b"
来源：http://hz.zdqjudy.top/gtokcndsxd.html

[T04] Kotlin：空安全
来源：http://hz.vqdsnc.cn/gtjjtkbsyb.html

val n: String? = null;  n?.length
来源：http://hz.cucudq.cn/gtbnberntl.html

[T05] Kotlin：when 表达式
来源：http://hz.shzxlz.cn/gtqnsfzgop.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.hfpthk.cn/gtuhfmfavt.html

[T06] Kotlin：集合映射
来源：http://hz.andypj.xyz/gtigzoakov.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.zhongyouzk.top/gtfilbowbk.html

[T07] Kotlin：集合过滤
来源：http://hz.fzhhl.top/gtbscmmkwn.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.zhoulong.xyz/gtjnesqbes.html

[T08] Kotlin：数据类
来源：http://hz.vqdsnc.cn/gtdkmhhidh.html

data class User(val name: String, val age: Int)
来源：http://hz.jinghuilouyu.cn/gtwabnuwsl.html


<!-- 参考信息 -->