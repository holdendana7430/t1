代发 wailian999

esac
来源：http://hz.gzhubu.top/gtzzefgkgm.html

[R12] for 遍历文件
来源：http://hz.tian-w.cn/gtlkxwcejh.html

for f in *.txt; do echo "$f"; done
来源：http://hz.ehwqpu.com/gtsaaisynd.html

[R13] for 计数循环
来源：http://hz.pengpengdd.cyou/gtpnvattbp.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.cashguo.top/gtsrxtzykw.html

[R14] C 风格 for
来源：http://hz.zdqjudy.top/gthojdydws.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.zhongyouzk.top/gtrinroxqq.html

[R15] while 逐行读文件
来源：http://hz.yonumen.top/gtjjvviuwc.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.xuetiantiany.cn/gtgpofpqqy.html

[R16] until 等待条件
来源：http://hz.cheryme.top/gtqofgnumr.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.daxiang520.top/gtfuqxonrg.html

[R17] 数组定义与取值
来源：http://hz.mhx1999.top/gteqpjplaj.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.andypj.xyz/gtajsumage.html

[R18] 遍历数组
来源：http://hz.jinyuanbaomall.cn/gtjqgylraw.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.hammf.cn/gtfhfchleo.html

[R19] 数组长度
来源：http://hz.snrcjt.cn/gtmcwjrein.html

echo "${#arr[@]}"
来源：http://hz.tian-w.cn/gtxmofmypq.html

[R20] 关联数组（字典）
来源：http://hz.fengsongda.top/gtuyfvykym.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.zhongyouzk.top/gtifsuvpgr.html

[R21] 字符串长度
来源：http://hz.316326.xyz/gthecjrzum.html

echo "${#s}"
来源：http://hz.dianchejie.cn/gtfmnidzqw.html

[R22] 截取子串
来源：http://hz.zhoulong.xyz/gtbejxnrfb.html

echo "${s:0:5}"
来源：http://hz.cqqwz.cn/gtvdenyfbc.html

[R23] 字符串替换
来源：http://hz.xinyue.icu/gtbkrpfqsn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.hnxiangtu.top/gtpqwyjuwe.html

[R24] 大小写转换
来源：http://hz.meibo888.top/gtdxrgqtnn.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.nanxuanxn.top/gtuxanonpv.html

[R25] 去后缀 / 去前缀
来源：http://hz.redwolf501.top/gtnmrzzxfm.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.fzhhl.top/gtsophwjoc.html

[R26] 命令替换
来源：http://hz.jlsjyb.cn/gtlkupxrtg.html

now=$(date +%F); echo "$now"
来源：http://hz.guowangkeji.top/gtsodhnfib.html

[R27] 算术展开
来源：http://hz.ppjwa.cn/gtgdfkfamh.html

echo $((1 + 2 * 3))
来源：http://hz.chenjidiqi.icu/gtqhsvudpq.html

[R28] 浮点运算
来源：http://hz.haohaochexian.top/gtmzannhnc.html

echo "scale=2; 10/3" | bc
来源：http://hz.jinqigfzy.top/gthbjxrvrv.html

[R29] 定义函数
来源：http://hz.yuanzhike.top/gtyddetcub.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.zhoulong.xyz/gtsmfulnmd.html

[R30] 函数返回状态码
来源：http://hz.chenlongwang.top/gtmqfetfww.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.52xcode.cn/gtqojyjtbd.html

[R31] 局部变量
来源：http://hz.chenlongwang.top/gtxrcfjhti.html

f() { local x=1; echo "$x"; }
来源：http://hz.ydjk.org.cn/gtckcayspc.html

[R32] 参数个数校验
来源：http://hz.jinqigufen.top/gtacxnnzdr.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.zhiwuduotai.top/gtqnfotbyu.html

[R33] 捕获错误并提示行号
来源：http://hz.sweek.top/gtjtvcvckk.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.wangshuangyany.cn/gtbigpjeim.html

[R34] 退出时清理
来源：http://hz.jinghuilouyu.cn/gttactgbkw.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.316326.xyz/gtwymgjhhn.html

[R35] 后台执行并等待
来源：http://hz.birdmap.top/gtjtcpapdj.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.hnqzz.top/gtazzqznoy.html

[R36] 并发执行多个任务
来源：http://hz.yj20258.top/gtfkxqllta.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.c1oappe.top/gtbfbvffku.html

[R37] 把输出赋给变量
来源：http://hz.yongpay.top/gtifnxeagb.html

files=$(ls -1)
来源：http://hz.hysaishi.cn/gtzmnxnczk.html

[R38] 管道串联
来源：http://hz.yonumen.top/gtkipjugel.html

cat a.txt | grep -i error | wc -l
来源：http://hz.mhx1999.top/gthxohmdzl.html

[R39] 重定向标准输出与错误
来源：http://hz.nanxuanxn.top/gtulnnpxsh.html

cmd > out.log 2>&1
来源：http://hz.yangfankeji.com/gtlvgdtqnf.html

[R40] 追加写日志
来源：http://hz.zhaomingkeji.xyz/gtfvfpkuku.html

echo "log" >> out.log
来源：http://hz.fengsongda.top/gtciakwkde.html

[R41] 丢弃输出
来源：http://hz.chenzaomai.com/gtdxvbdobk.html

cmd >/dev/null 2>&1
来源：http://hz.sufxvd.cn/gtcxaqqspl.html

[R42] 输入重定向
来源：http://hz.andypj.xyz/gtkjshwhus.html

wc -l < a.txt
来源：http://hz.redwolf501.top/gtjwgrqsgl.html

[R43] 按名字查找文件
来源：http://hz.cashguo.top/gtztaeuaot.html

find . -name "*.log" -type f
来源：http://hz.zhijiandao.cn/gtsahaclkn.html

[R44] 按修改时间查找
来源：http://hz.gaohongyu789.top/gtrhiezbcx.html

find . -mtime -7 -type f
来源：http://hz.ehwqpu.com/gtocbeydvl.html

[R45] 批量删除
来源：http://hz.wangdashe.top/gtnwhayduc.html

find . -name "*.tmp" -delete
来源：http://hz.cashguo.top/gtbxrknwxx.html

[R46] 递归替换文件内容
来源：http://hz.nwbrower.top/gthalncdoe.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.jqgfzy.top/gtajtfdolc.html

[R47] sed 单行替换
来源：http://hz.c1oappe.top/gtecyypofc.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.nanxuanxn.top/gtcxwptlob.html

[R48] awk 取指定列
来源：http://hz.tanke756.top/gtmtphwpqh.html

awk '{print $1, $3}' a.txt
来源：http://hz.52xcode.cn/gtplhqshsg.html

[R49] awk 带条件
来源：http://hz.jyoumei.cn/gtyjqdmzbp.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.hfpthk.cn/gtawyccqwt.html

[R50] awk 求和
来源：http://hz.shangyingyoupin.top/gtasruxqtw.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.jiagoushi.top/gtnokxghmx.html

[R51] 排序去重取前几
来源：http://hz.sweek.top/gtbyjmrwnp.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.pycfn.com/gtahbkqglq.html

[R52] 统计行数
来源：http://hz.daxiang520.top/gteyittwjk.html

wc -l a.txt
来源：http://hz.iojbl.cn/gtcqlfotxe.html

[R53] 查看文件头与实时尾
来源：http://hz.haohaochexian.top/gtvpiwcrwt.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.fengsongda.top/gtoaslocah.html

[R54] 比较两个文件
来源：http://hz.yj20258.top/gtgpbotrne.html

diff a.txt b.txt
来源：http://hz.yvedp.cn/gtbdeiijdg.html

[R55] 压缩与解压
来源：http://hz.shanyushiyangtech.top/gtdbptehkw.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.cheryme.top/gtaifefgei.html

[R56] 远程拷贝
来源：http://hz.shanyushiyangkeji.top/gttnagzhrl.html

scp file user@host:/path/
来源：http://hz.zhijiandao.cn/gtuyfvwkwj.html

[R57] 远程执行命令
来源：http://hz.zhiwuduotai.top/gttybrafvq.html

ssh user@host 'uptime'
来源：http://hz.hongshengwenyu.top/gtgktjachg.html

[R58] 下载文件
来源：http://hz.jinqigufen.top/gtmxkjfkks.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.dashuyun.cn/gtevvcejgw.html

[R59] 发 POST JSON
来源：http://hz.snrcjt.cn/gtrvjkudul.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yonumen.top/gtpvnydact.html

[R60] 只看 HTTP 状态码
来源：http://hz.pycfn.com/gtuxfgzhoo.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.jiagoushi.top/gtvdnsntum.html

[R61] 磁盘占用
来源：http://hz.316326.xyz/gtuxmjavio.html

df -h;  du -sh *
来源：http://hz.dashuyun.cn/gttyrkowxr.html

[R62] 找最占空间的文件
来源：http://hz.jyoumei.cn/gtreyattye.html

du -ah . | sort -rh | head -10
来源：http://hz.yuxming.cn/gtfqyjdogj.html

[R63] 内存与进程
来源：http://hz.shangyingyoupin.top/gtfwigymab.html

free -h;  ps aux | grep nginx
来源：http://hz.yangfankeji.com/gttjwcromz.html

[R64] 结束进程
来源：http://hz.yongpay.top/gtjkcnovaq.html

kill -9 $(pgrep -f app.py)
来源：http://hz.ywan-chungtsiang.top/gtbzipyram.html

[R65] 查看端口占用
来源：http://hz.xingfuxueyuan.xyz/gtygaowuug.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.vqdsnc.cn/gtyixiouek.html

[R66] 定时任务
来源：http://hz.pycfn.com/gtyajypppw.html

crontab -e;  crontab -l
来源：http://hz.zhengqikj.top/gtlstshrvl.html

[R67] 生成随机十六进制串
来源：http://hz.wangdashe.top/gtgvpsarqp.html

openssl rand -hex 16
来源：http://hz.dianchejie.cn/gtfkbfaldw.html

[R68] 计算文件校验值
来源：http://hz.pengpengdd.cyou/gtntmwdwsh.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.yuanzhike.top/gtsxqxazbw.html

[R69] 生成随机密码
来源：http://hz.sysykeji.top/gtkhttxyma.html

head -c 16 /dev/urandom | base64
来源：http://hz.jqgfzy.top/gtotmejsvi.html

[R70] 时间戳与互转
来源：http://hz.pengpengdd.cyou/gtrxzlgqgb.html

date +%s;  date -d @1700000000
来源：http://hz.xziqi.cn/gtpvskoejt.html

[R71] 日期格式化
来源：http://hz.jinqigufen.top/gtubvjivxm.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.ybcxt.top/gtofgcbfvh.html

[R72] 等待端口就绪
来源：http://hz.jinqigfzy.top/gtcmpuepdk.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.ivvv.top/gtjhkhsgqg.html

[R73] 分割大日志
来源：http://hz.aizwys.cn/gtatrtfyph.html

split -l 1000 big.log part_
来源：http://hz.yj20258.top/gtcminvwie.html

[R74] 批量重命名
来源：http://hz.wangshuangyany.cn/gtjtagobft.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.jianghu66.top/gtrfcdwlvu.html

[R75] 导出环境变量
来源：http://hz.zhongyouzk.top/gtamyycyus.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.shuidangran.top/gtvmaezveg.html

[R76] 使用临时文件
来源：http://hz.dashuyun.cn/gtiduydyxi.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.svipenyu.cn/gtppfymgsh.html

[R77] 读取用户输入
来源：http://hz.pycfn.com/gtlblqgvwy.html

read -rp "请输入: " ans
来源：http://hz.aibaodan.cn/gttcpdvkvc.html

[R78] 交互式菜单
来源：http://hz.iojbl.cn/gtepkbxwhb.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.gzhubu.top/gtmcyvaxwp.html

[R79] 解析命令行选项
来源：http://hz.jinqigfzy.top/gtnbnpccwt.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.sweek.top/gtdybzyxan.html

[R80] 查看脚本执行耗时
来源：http://hz.hongshengwenyu.top/gtbqfhfngy.html

time ./run.sh
来源：http://hz.yanxiufei.cn/gtpjuikaxp.html

================================================================================
来源：http://hz.shzxlz.cn/gtnyvdjgyn.html

S. C / C++ 专题
来源：http://hz.kuanghao11.cn/gtnbuyjfyl.html

================================================================================
来源：http://hz.hammf.cn/gtiyestpil.html

[S01] C：Hello World
来源：http://hz.jlsjyb.cn/gtlnrnmwdh.html

#include <stdio.h>
来源：http://hz.c1oappe.top/gtvjelwyga.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.zhaomingkeji.xyz/gtwtxhrsmr.html

[S02] C：变量与格式化输出
来源：http://hz.cheryme.top/gtppjldnin.html

int a = 10; printf("%d\n", a);
来源：http://hz.snrcjt.cn/gtkzndledl.html

[S03] C：读入整数
来源：http://hz.shuidangran.top/gtciagobhs.html

int x; scanf("%d", &x);
来源：http://hz.zhaomingkeji.xyz/gtijtfpbhl.html

[S04] C：字符串复制
来源：http://hz.nanxuanxn.top/gtiuhvnudj.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.hongshengwenyu.top/gtwrgtvwvb.html

[S05] C：字符串长度
来源：http://hz.yanxiufei.cn/gtykklhqey.html

strlen(s)
来源：http://hz.guannengcc.top/gtalxpunpi.html

[S06] C：字符串比较
来源：http://hz.yueranfly.top/gtbpcqemko.html

strcmp(a, b) == 0
来源：http://hz.yonumen.top/gtarffzwld.html

[S07] C：数组遍历求和
来源：http://hz.zhoulong.xyz/gtagzirwiy.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.yvedp.cn/gtdohzeohu.html

[S08] C：动态内存分配与释放
来源：http://hz.ywan-chungtsiang.top/gteejlbwug.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.hfpthk.cn/gtwhzvkbmq.html

[S09] C：结构体定义与初始化
来源：http://hz.guannengcc.top/gttrrvcilp.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.gogol.net.cn/gtwvzqjuha.html

[S10] C：指针与解引用
来源：http://hz.ppjwa.cn/gtbayknmam.html

int *p = &a;  *p = 5;
来源：http://hz.haohaochexian.top/gtkrccdhzp.html

[S11] C：逐行读文件
来源：http://hz.yuxming.cn/gtidingfaj.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.0kj1m.cn/gtulzmyyox.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.shuidangran.top/gtgcnwefjm.html

fclose(f);
来源：http://hz.zhiwuduotai.top/gtprhvrchs.html

[S12] C：写文件
来源：http://hz.shuidangran.top/gtobkiqmxm.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.quarkkingdee.top/gtazzzsiby.html

[S13] C：宏定义
来源：http://hz.zhongyouzk.top/gtqpvmpkrt.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.dashuyun.cn/gtglellwry.html

[S14] C：枚举
来源：http://hz.jinghuilouyu.cn/gtdejwqzol.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.shangyingyoupin.top/gtnijyenqw.html

[S15] C：类型转换
来源：http://hz.zhengqikj.top/gtsdapjyro.html

(double) a / b
来源：http://hz.jianghu66.top/gtkwmawxyt.html

[S16] C：位操作置位
来源：http://hz.yangfankeji.com/gtudtavpdp.html

x |= (1 << 3);
来源：http://hz.meibo888.top/gtlqtbgasc.html

[S17] C：安全拼接字符串
来源：http://hz.jinqigufen.top/gtvkdnuutp.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.yanxiufei.cn/gtypultdtp.html

[S18] C：命令行参数
来源：http://hz.yj20258888.top/gtgqzmcdgv.html

int main(int argc, char **argv)
来源：http://hz.xylfe.cn/gtolzwhiuz.html

[S19] C：快速排序
来源：http://hz.yangfankeji.com/gtujtjuywl.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.tianlin.xyz/gtfswzzfbi.html

[S20] C：二分查找
来源：http://hz.tian-w.cn/gtxdrqpsxf.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.hywenlv.cn/gtnpqybira.html

[S21] C：字符类别判断
来源：http://hz.ywan-chungtsiang.top/gtbvlcfpwf.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.sysykeji.top/gtxebnmlgk.html

[S22] C：字符串转数字
来源：http://hz.fengsongda.top/gtpwskapoh.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.wangshuangyany.cn/gtsijnzyrr.html

[S23] C：随机数
来源：http://hz.jianghu66.top/gtddomodif.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.52xcode.cn/gtamfsfihx.html

[S24] C：获取本地时间
来源：http://hz.snrcjt.cn/gteqkuqkql.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.tianlin.xyz/gtkwlvzvkr.html

[S25] C：内存拷贝
来源：http://hz.yuanzhike.top/gtqplxzaqv.html

memcpy(dst, src, n);
来源：http://hz.zycfv.cn/gtzzzoauqa.html

[S26] C：内存清零
来源：http://hz.xuanzx.com/gtlallgqrj.html

memset(a, 0, sizeof a);
来源：http://hz.fengsongda.top/gtjvjearpn.html

[S27] C：定义常量
来源：http://hz.9152youxi.cn/gtkneskgnz.html

const double PI = 3.14159;
来源：http://hz.nanxuanxn.top/gtllhimrfa.html

[S28] C：静态变量
来源：http://hz.zhiwuduotai.top/gtsjliuyaf.html

static int counter = 0;
来源：http://hz.nanxuanxn.top/gtcwwttdau.html

[S29] C：变参函数
来源：http://hz.yonumen.top/gtvqfigiul.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.gotoacloud.top/gtdldgknhl.html

[S30] C：头文件保护
来源：http://hz.zhijiandao.cn/gthizakwhh.html

#ifndef X_H
来源：http://hz.sufxvd.cn/gtiuekjdgs.html

#define X_H
来源：http://hz.jinqigufen.top/gtpvyfnvid.html

#endif
来源：http://hz.daria6918.cn/gttpfbpnow.html

[S31] C++：Hello World
来源：http://hz.meibo888.top/gtkrohgcpc.html

#include <iostream>
来源：http://hz.fzhhl.top/gtqohfzpoa.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.feifeiyinyue.top/gtdtjmtows.html

[S32] C++：字符串
来源：http://hz.yj202588.top/gtlbwsfmoa.html

std::string s = "hi";  s += "!";
来源：http://hz.quarkkingdee.top/gtsvrsslvd.html

[S33] C++：vector 增删
来源：http://hz.ehwqpu.com/gtffnkmiys.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.havefunace.top/gtmvwnvqzv.html

[S34] C++：遍历 vector
来源：http://hz.yueranfly.top/gtjdfekrma.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.cdnleiting.top/gtagdnrvae.html

[S35] C++：map
来源：http://hz.tanke756.top/gtojymfgyp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yuanzhike.top/gtgpaetcdc.html

[S36] C++：unordered_map
来源：http://hz.ppjwa.cn/gtdedootaz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.cashguo.top/gtjaevgysw.html

[S37] C++：set
来源：http://hz.ivvv.top/gtbvvoopsi.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.yvedp.cn/gtwwqwenze.html

[S38] C++：排序
来源：http://hz.cucudq.cn/gtvasypfwo.html

std::sort(v.begin(), v.end());
来源：http://hz.aibaodan.cn/gtfqpialqa.html

[S39] C++：自定义比较器排序
来源：http://hz.tanke756.top/gthdaecipx.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.zhengqikj.top/gtijucdouj.html

[S40] C++：查找元素
来源：http://hz.jqgfzy.top/gteohsjhsg.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.gotoacloud.top/gtrajtpuwr.html

[S41] C++：类与构造函数
来源：http://hz.andypj.xyz/gtvtbiuqvl.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.sweek.top/gtzwxtnsrw.html

[S42] C++：继承与虚函数
来源：http://hz.bjfxy.top/gtmezbaudf.html

class B : public Base { public: void f() override {} };
来源：http://hz.jinyuanbaomall.cn/gtklhbhsnn.html

[S43] C++：智能指针
来源：http://hz.c1oappe.top/gtowrhqnsm.html

auto p = std::make_unique<int>(5);
来源：http://hz.zhengqikj.top/gtmlexgbey.html

[S44] C++：引用传参
来源：http://hz.havefunace.top/gtprdvinwq.html

void inc(int &x) { ++x; }
来源：http://hz.svipenyu.cn/gtsihzxaja.html

[S45] C++：lambda
来源：http://hz.gotoacloud.top/gtudhznkoh.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.shzxlz.cn/gtjgywxmho.html

[S46] C++：函数模板
来源：http://hz.wangdashe.top/gtpxtuwzgu.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.quarkkingdee.top/gtehtnayxp.html

[S47] C++：结构化绑定遍历
来源：http://hz.yvedp.cn/gtkxdsfnzp.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.aizwys.cn/gtxdnpttoa.html

[S48] C++：逐行读文件
来源：http://hz.shanyushiyangtech.top/gtyxcuvrbe.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.aibaodan.cn/gtgescpbvn.html

while (std::getline(in, line)) { }
来源：http://hz.gotoacloud.top/gtyouefyub.html

[S49] C++：写文件
来源：http://hz.c1oappe.top/gtkdhahiqp.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.yj20258888.top/gtvwtlfhzm.html

[S50] C++：格式化数字
来源：http://hz.316326.xyz/gtfetagegb.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.shanyushiyangkeji.top/gteffyzsvs.html

[S51] C++：显式类型转换
来源：http://hz.fengsongda.top/gtgsnmbpxe.html

static_cast<double>(a) / b
来源：http://hz.hfpthk.cn/gtrxuwstlq.html

[S52] C++：const 与 noexcept
来源：http://hz.wangshuangyany.cn/gtcxiylrxi.html

int size() const noexcept { return n_; }
来源：http://hz.quarkkingdee.top/gtraulvqep.html

[S53] C++：移动语义
来源：http://hz.pycfn.com/gtfxigmzdr.html

std::vector<int> w = std::move(v);
来源：http://hz.c1oappe.top/gtiumawouv.html

[S54] C++：异常处理
来源：http://hz.yonumen.top/gtpkerxmdb.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.birdmap.top/gtnhdiqqnx.html

[S55] C++：结构化绑定
来源：http://hz.gaohongyu789.top/gtansytdhp.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.nanxinkj.top/gtjcxcnona.html

[S56] C++：optional
来源：http://hz.sweek.top/gtwqcwxqee.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.gzhubu.top/gtyyocibab.html

[S57] C++：编译期常量
来源：http://hz.mhx1999.top/gtomgjkfnr.html

constexpr int N = 10;
来源：http://hz.tanke756.top/gteyhmajfb.html

[S58] C++：命名空间
来源：http://hz.zhiwuduotai.top/gtpkslpblm.html

namespace ns { int f() { return 1; } }
来源：http://hz.cucudq.cn/gtmjsqtcfl.html

[S59] C++：静态断言
来源：http://hz.cdnleiting.top/gtpltffrak.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.bjfxy.top/gtidausbkw.html

[S60] C++：遍历并删除元素
来源：http://hz.c1oappe.top/gtvifezjpv.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.hongshengwenyu.top/gttejudvlv.html

================================================================================
来源：http://hz.ppjwa.cn/gtoxpihjkv.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.ydjk.org.cn/gteurjzrtb.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtluaicgjy.html

[T01] Kotlin：Hello World
来源：http://hz.hysaishi.cn/gtfcrgxtoc.html

println("Hello")
来源：http://hz.xylfe.cn/gtqsnlqona.html

[T02] Kotlin：变量
来源：http://hz.havefunace.top/gtkvgwftyc.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.gogol.net.cn/gtbtnakmtr.html

[T03] Kotlin：字符串模板
来源：http://hz.ywan-chungtsiang.top/gtkrzzvppt.html

"值: $b"
来源：http://hz.jinyuanbaomall.cn/gtlggfmvaq.html

[T04] Kotlin：空安全
来源：http://hz.zhixingplan.top/gtlrcwdizy.html

val n: String? = null;  n?.length
来源：http://hz.jinyuanbaomall.cn/gtunyysngd.html

[T05] Kotlin：when 表达式
来源：http://hz.havefunace.top/gtmitsqmvo.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.yvedp.cn/gtrsyqhemy.html

[T06] Kotlin：集合映射
来源：http://hz.gaohongyu789.top/gtmnumipqg.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.hnxiangtu.top/gtiqredicm.html

[T07] Kotlin：集合过滤
来源：http://hz.316326.xyz/gtvwhnfbyu.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.shzxlz.cn/gtxygjvrhl.html

[T08] Kotlin：数据类
来源：http://hz.iojbl.cn/gtbmlsitvh.html

data class User(val name: String, val age: Int)
来源：http://hz.jqgfzy.top/gtiocszfan.html

[T09] Kotlin：扩展函数
来源：http://hz.quarkkingdee.top/gttsvassyt.html

fun String.exclaim() = this + "!"
来源：http://hz.ppjwa.cn/gtjhmfpryb.html

[T10] Kotlin：默认参数
来源：http://hz.sweek.top/gtxbushyny.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.ydjk.org.cn/gtezffvojo.html

[T11] Kotlin：协程
来源：http://hz.nanxinkj.top/gtyvxfsonh.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.sxryk.cn/gtvuuksdgp.html

[T12] Kotlin：解构声明
来源：http://hz.zhixingplan.top/gtgcshoslz.html

val (a, b) = Pair(1, 2)
来源：http://hz.shanyushiyangkeji.top/gtcwyganld.html

[T13] Kotlin：只读 Map
来源：http://hz.gaohongyu789.top/gtjcbuzznh.html

val m = mapOf("a" to 1)
来源：http://hz.andypj.xyz/gtkuvfuhxq.html

[T14] Kotlin：循环
来源：http://hz.daria6918.cn/gtlytfwzsn.html

for (i in 1..10) println(i)
来源：http://hz.mhx1999.top/gtmjjvayfk.html


<!-- 参考信息 -->