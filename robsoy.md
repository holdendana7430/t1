代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://hz.chenlongwang.top/gtrkgobsdc.html

[R14] C 风格 for
来源：http://hz.jinghuilouyu.cn/gtwnianqgs.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.iojbl.cn/gttuqddnxf.html

[R15] while 逐行读文件
来源：http://hz.zhijiandao.cn/gtujywzyad.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.daxiang520.top/gtjpueusgn.html

[R16] until 等待条件
来源：http://hz.jinghuilouyu.cn/gtinqjnftp.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.haohaochexian.top/gtdbcwectd.html

[R17] 数组定义与取值
来源：http://hz.shangyingyoupin.top/gtpsmkbuln.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.hongshengwenyu.top/gtmbhmxonl.html

[R18] 遍历数组
来源：http://hz.vqdsnc.cn/gtguexvbvf.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.haohaochexian.top/gttnjqltcv.html

[R19] 数组长度
来源：http://hz.vqdsnc.cn/gtzcxxbkrj.html

echo "${#arr[@]}"
来源：http://hz.yj20258.top/gtnuwdiqlx.html

[R20] 关联数组（字典）
来源：http://hz.jqgufenzy.top/gtoszxjwxi.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.shzxlz.cn/gtdparjpwh.html

[R21] 字符串长度
来源：http://hz.fengsongda.top/gtylvyqwur.html

echo "${#s}"
来源：http://hz.jinyuanbaomall.cn/gtlyibbahv.html

[R22] 截取子串
来源：http://hz.feifeiyinyue.top/gtguldqqrd.html

echo "${s:0:5}"
来源：http://hz.52xcode.cn/gtmftjgelu.html

[R23] 字符串替换
来源：http://hz.quarkkingdee.top/gtbquuxeof.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.cheryme.top/gtsdmqcdtl.html

[R24] 大小写转换
来源：http://hz.jqgfzy.top/gtoguhbfge.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.daxiang520.top/gthtctadoj.html

[R25] 去后缀 / 去前缀
来源：http://hz.yvedp.cn/gtuwepmpez.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.hywenlv.cn/gtdlkeggbs.html

[R26] 命令替换
来源：http://hz.jinqigfzy.top/gtjkruqtbp.html

now=$(date +%F); echo "$now"
来源：http://hz.0kj1m.cn/gtujudhmhk.html

[R27] 算术展开
来源：http://hz.yuxming.cn/gtfjvkocyh.html

echo $((1 + 2 * 3))
来源：http://hz.zycfv.cn/gtvzrgacom.html

[R28] 浮点运算
来源：http://hz.daria6918.cn/gtdkbuiqvy.html

echo "scale=2; 10/3" | bc
来源：http://hz.yueranfly.top/gtwmzyyxjg.html

[R29] 定义函数
来源：http://hz.vqdsnc.cn/gtgbmjdskm.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.redwolf501.top/gttfpfgjmq.html

[R30] 函数返回状态码
来源：http://hz.zhongyouzk.top/gtlpclnuvf.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.jinghuilouyu.cn/gticegwpse.html

[R31] 局部变量
来源：http://hz.gzhubu.top/gtwzyqijbk.html

f() { local x=1; echo "$x"; }
来源：http://hz.zycfv.cn/gtysimodwc.html

[R32] 参数个数校验
来源：http://hz.kuanghao11.cn/gtbzivterz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.cucudq.cn/gtfdsinkme.html

[R33] 捕获错误并提示行号
来源：http://hz.fengsongda.top/gtniwhqpjq.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.pengpengdd.cyou/gtouzhdkws.html

[R34] 退出时清理
来源：http://hz.yongpay.top/gtctifglgw.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.wangdashe.top/gtrbzljfew.html

[R35] 后台执行并等待
来源：http://hz.guowangkeji.top/gtowvqfptt.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.chenzaomai.com/gtxpdpdbgh.html

[R36] 并发执行多个任务
来源：http://hz.xuanzx.com/gtchyllyve.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.quarkkingdee.top/gtqixoagdl.html

[R37] 把输出赋给变量
来源：http://hz.vqdsnc.cn/gtmszgvptq.html

files=$(ls -1)
来源：http://hz.jinyuanbaomall.cn/gtqpiqgtji.html

[R38] 管道串联
来源：http://hz.zhiwuduotai.top/gtgwpbpwvi.html

cat a.txt | grep -i error | wc -l
来源：http://hz.daria6918.cn/gtgxkxlscn.html

[R39] 重定向标准输出与错误
来源：http://hz.shanyushiyangtech.top/gttmmlhzhn.html

cmd > out.log 2>&1
来源：http://hz.haohaochexian.top/gtsmngsekf.html

[R40] 追加写日志
来源：http://hz.cqqwz.cn/gtflftdudr.html

echo "log" >> out.log
来源：http://hz.gaohongyu789.top/gtpltavdhg.html

[R41] 丢弃输出
来源：http://hz.xuetiantiany.cn/gtufzftinb.html

cmd >/dev/null 2>&1
来源：http://hz.havefunace.top/gtnpngomju.html

[R42] 输入重定向
来源：http://hz.52xcode.cn/gtkigfbgmc.html

wc -l < a.txt
来源：http://hz.andypj.xyz/gtwlqlsbxm.html

[R43] 按名字查找文件
来源：http://hz.52xcode.cn/gtstuntvxk.html

find . -name "*.log" -type f
来源：http://hz.zhoulong.xyz/gtbjhsuhhw.html

[R44] 按修改时间查找
来源：http://hz.9152youxi.cn/gthbqohvwm.html

find . -mtime -7 -type f
来源：http://hz.shanyushiyangkeji.top/gtaqposwyi.html

[R45] 批量删除
来源：http://hz.tianlin.xyz/gtyyhxuirn.html

find . -name "*.tmp" -delete
来源：http://hz.aibaodan.cn/gtzxdudfwj.html

[R46] 递归替换文件内容
来源：http://hz.zhongyouzk.top/gtikzerpls.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.zhixingplan.top/gtdezajtvq.html

[R47] sed 单行替换
来源：http://hz.0kj1m.cn/gtibkweipe.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.havefunace.top/gtjxjxguaf.html

[R48] awk 取指定列
来源：http://hz.yuxming.cn/gtclwcylln.html

awk '{print $1, $3}' a.txt
来源：http://hz.xziqi.cn/gtqibivcul.html

[R49] awk 带条件
来源：http://hz.hysaishi.cn/gtpjbrveat.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.sufxvd.cn/gtejwsxfhh.html

[R50] awk 求和
来源：http://hz.jinqigufen.top/gtfzuyyczb.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.c1oappe.top/gtemxurrei.html

[R51] 排序去重取前几
来源：http://hz.birdmap.top/gtsxipckiw.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.gogol.net.cn/gtvqlicnpy.html

[R52] 统计行数
来源：http://hz.yonumen.top/gtvnbwucde.html

wc -l a.txt
来源：http://hz.nwbrower.top/gtzczsmngs.html

[R53] 查看文件头与实时尾
来源：http://hz.quarkkingdee.top/gtaghwvwmr.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.guannengcc.top/gtqdragczm.html

[R54] 比较两个文件
来源：http://hz.ppjwa.cn/gtzazojyqp.html

diff a.txt b.txt
来源：http://hz.zycfv.cn/gtmzlkgejw.html

[R55] 压缩与解压
来源：http://hz.yuxming.cn/gtmtmmdbja.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.havefunace.top/gthxfxhwoo.html

[R56] 远程拷贝
来源：http://hz.haohaochexian.top/gtmgyisjki.html

scp file user@host:/path/
来源：http://hz.9152youxi.cn/gtfhhvdlpe.html

[R57] 远程执行命令
来源：http://hz.sxryk.cn/gtqomypzmt.html

ssh user@host 'uptime'
来源：http://hz.hysaishi.cn/gttdljheyr.html

[R58] 下载文件
来源：http://hz.cashguo.top/gtbygaknlr.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.dashuyun.cn/gtdhodiwvt.html

[R59] 发 POST JSON
来源：http://hz.mhx1999.top/gtoowbnelz.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.hammf.cn/gtydphigbk.html

[R60] 只看 HTTP 状态码
来源：http://hz.chenlongwang.top/gtppiezfcn.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.gzhubu.top/gtbkggcltj.html

[R61] 磁盘占用
来源：http://hz.nwbrower.top/gtpzqbnobx.html

df -h;  du -sh *
来源：http://hz.jlsjyb.cn/gtbofeebsz.html

[R62] 找最占空间的文件
来源：http://hz.gaohongyu789.top/gthgwbfobp.html

du -ah . | sort -rh | head -10
来源：http://hz.zhiwuduotai.top/gttflfygve.html

[R63] 内存与进程
来源：http://hz.xingfuxueyuan.xyz/gtxqcbyaqs.html

free -h;  ps aux | grep nginx
来源：http://hz.wangdashe.top/gtjbhxnvff.html

[R64] 结束进程
来源：http://hz.ydzc1.top/gtykvnthlt.html

kill -9 $(pgrep -f app.py)
来源：http://hz.yuanzhike.top/gtjtyykxic.html

[R65] 查看端口占用
来源：http://hz.wangdashe.top/gtavnyezuz.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.shuidangran.top/gtdnrpobqs.html

[R66] 定时任务
来源：http://hz.ppjwa.cn/gtpyrwyrqa.html

crontab -e;  crontab -l
来源：http://hz.wangshuangyany.cn/gtndyjbaxx.html

[R67] 生成随机十六进制串
来源：http://hz.zdqjudy.top/gttzhfrcxz.html

openssl rand -hex 16
来源：http://hz.jlsjyb.cn/gtlkhkibbo.html

[R68] 计算文件校验值
来源：http://hz.hammf.cn/gtgbhqxolo.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.zhengqikj.top/gttebuvyyj.html

[R69] 生成随机密码
来源：http://hz.shzxlz.cn/gtntnfssmn.html

head -c 16 /dev/urandom | base64
来源：http://hz.yj20258.top/gtwphhyznx.html

[R70] 时间戳与互转
来源：http://hz.aizwys.cn/gticnblwgu.html

date +%s;  date -d @1700000000
来源：http://hz.jiagoushi.top/gtogypszms.html

[R71] 日期格式化
来源：http://hz.yonumen.top/gtfrksrpts.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.ydjk.org.cn/gtsdgmabbv.html

[R72] 等待端口就绪
来源：http://hz.jlsjyb.cn/gthjajgovl.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.c1oappe.top/gtokpnkdck.html

[R73] 分割大日志
来源：http://hz.xuetiantiany.cn/gtnoplevce.html

split -l 1000 big.log part_
来源：http://hz.jqgfzy.top/gtnjblwbpv.html

[R74] 批量重命名
来源：http://hz.aizwys.cn/gtymueecfc.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.chenlongwang.top/gtxywosyup.html

[R75] 导出环境变量
来源：http://hz.yangfankeji.com/gtrmenbnsk.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.zdqjudy.top/gtktzzwiyb.html

[R76] 使用临时文件
来源：http://hz.yonumen.top/gtlzqjlumm.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.yonumen.top/gthtrpjicp.html

[R77] 读取用户输入
来源：http://hz.ydjk.org.cn/gtnnaxbeoe.html

read -rp "请输入: " ans
来源：http://hz.xingfuxueyuan.xyz/gtcmnvghut.html

[R78] 交互式菜单
来源：http://hz.cheryme.top/gtefylwjuo.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.shzxlz.cn/gtoxybjtuy.html

[R79] 解析命令行选项
来源：http://hz.xinyue.icu/gtkixwrfos.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.shanyushiyangtech.top/gtbpaxczyu.html

[R80] 查看脚本执行耗时
来源：http://hz.fzhhl.top/gtggpomdfd.html

time ./run.sh
来源：http://hz.shzxlz.cn/gtvyvdmkiv.html

================================================================================
来源：http://hz.gogol.net.cn/gtwcjmuvhb.html

S. C / C++ 专题
来源：http://hz.xziqi.cn/gtmwljxazp.html

================================================================================
来源：http://hz.meibo888.top/gtxxnhbcjz.html

[S01] C：Hello World
来源：http://hz.zhixingplan.top/gtajymuyhz.html

#include <stdio.h>
来源：http://hz.svipenyu.cn/gtkprotuyp.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.tian-w.cn/gtdyhvrgoa.html

[S02] C：变量与格式化输出
来源：http://hz.ydzc1.top/gtqmcsvnxo.html

int a = 10; printf("%d\n", a);
来源：http://hz.gotoacloud.top/gtlagpumcn.html

[S03] C：读入整数
来源：http://hz.sweek.top/gtqakwymqj.html

int x; scanf("%d", &x);
来源：http://hz.haohaochexian.top/gtldbqhgpd.html

[S04] C：字符串复制
来源：http://hz.mhx1999.top/gtjuvgczqq.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.sysykeji.top/gtgzrqedlp.html

[S05] C：字符串长度
来源：http://hz.pengpengdd.cyou/gtzhczinbq.html

strlen(s)
来源：http://hz.xuetiantiany.cn/gtkehcpdyc.html

[S06] C：字符串比较
来源：http://hz.aizwys.cn/gtsnjyaowm.html

strcmp(a, b) == 0
来源：http://hz.yueranfly.top/gtbwatxrlz.html

[S07] C：数组遍历求和
来源：http://hz.shangyingyoupin.top/gtnplrrzdn.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.ivvv.top/gtczegziwb.html

[S08] C：动态内存分配与释放
来源：http://hz.fzhhl.top/gtvhtdsqib.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.yangfankeji.com/gtxyygwcth.html

[S09] C：结构体定义与初始化
来源：http://hz.chenzaomai.com/gtcwvhciow.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.yonumen.top/gtgfctvhbw.html

[S10] C：指针与解引用
来源：http://hz.shangyingyoupin.top/gtifevfnlz.html

int *p = &a;  *p = 5;
来源：http://hz.aibaodan.cn/gtsfpvajce.html

[S11] C：逐行读文件
来源：http://hz.hammf.cn/gtikinllro.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.dianchejie.cn/gtjtmohtmt.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.shanyushiyangtech.top/gthuixjcij.html

fclose(f);
来源：http://hz.cashguo.top/gtsbokojnv.html

[S12] C：写文件
来源：http://hz.daria6918.cn/gtanuzulnn.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.hnqzz.top/gtfetmlwff.html

[S13] C：宏定义
来源：http://hz.jinghuilouyu.cn/gtijqawjyy.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.zhiwuduotai.top/gtzvvovmir.html

[S14] C：枚举
来源：http://hz.ywan-chungtsiang.top/gtaipgcjae.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.pycfn.com/gtbtvpozmz.html

[S15] C：类型转换
来源：http://hz.guowangkeji.top/gtedjmbjsq.html

(double) a / b
来源：http://hz.jianghu66.top/gtfepbutag.html

[S16] C：位操作置位
来源：http://hz.ywan-chungtsiang.top/gtkoavagry.html

x |= (1 << 3);
来源：http://hz.ppjwa.cn/gtmwjrclaq.html

[S17] C：安全拼接字符串
来源：http://hz.mhx1999.top/gtprtxdkrw.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.52xcode.cn/gtbugsyyaa.html

[S18] C：命令行参数
来源：http://hz.jinghuilouyu.cn/gtpqrdjsuh.html

int main(int argc, char **argv)
来源：http://hz.yvedp.cn/gtollfkmac.html

[S19] C：快速排序
来源：http://hz.shuidangran.top/gtirpcdqvz.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.jianghu66.top/gtzkcydvtx.html

[S20] C：二分查找
来源：http://hz.cheryme.top/gtbeetbukz.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.birdmap.top/gtrvfbnaxc.html

[S21] C：字符类别判断
来源：http://hz.meibo888.top/gtrkgmucqq.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.dashuyun.cn/gtlewoqcdr.html

[S22] C：字符串转数字
来源：http://hz.yonumen.top/gtdwdhahsq.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.shangyingyoupin.top/gttexpbutb.html

[S23] C：随机数
来源：http://hz.ydzc1.top/gttvajselb.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.tian-w.cn/gtvlqydeuw.html

[S24] C：获取本地时间
来源：http://hz.cucudq.cn/gtumektpgm.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.daria6918.cn/gtjybiythp.html

[S25] C：内存拷贝
来源：http://hz.cucudq.cn/gtinhxmqas.html

memcpy(dst, src, n);
来源：http://hz.shanyushiyangkeji.top/gtghezoalu.html

[S26] C：内存清零
来源：http://hz.dianchejie.cn/gtxdyhzztb.html

memset(a, 0, sizeof a);
来源：http://hz.hnxiangtu.top/gtiwtxrvft.html

[S27] C：定义常量
来源：http://hz.quarkkingdee.top/gtwchzghym.html

const double PI = 3.14159;
来源：http://hz.zhaomingkeji.xyz/gtwlqchnwz.html

[S28] C：静态变量
来源：http://hz.xuetiantiany.cn/gtpvqumerw.html

static int counter = 0;
来源：http://hz.yj20258888.top/gtjsylnnyi.html

[S29] C：变参函数
来源：http://hz.cheryme.top/gtgizuknyt.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.sysykeji.top/gtrucllpdn.html

[S30] C：头文件保护
来源：http://hz.hysaishi.cn/gttzfefonj.html

#ifndef X_H
来源：http://hz.svipenyu.cn/gtsxupdsjs.html

#define X_H
来源：http://hz.zhaomingkeji.xyz/gtyppumflb.html

#endif
来源：http://hz.jyoumei.cn/gtuhinsznb.html

[S31] C++：Hello World
来源：http://hz.tian-w.cn/gtjjjmgbcn.html

#include <iostream>
来源：http://hz.gaohongyu789.top/gtxfexaanz.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.shangyingyoupin.top/gthnfxvvrh.html

[S32] C++：字符串
来源：http://hz.shuidangran.top/gtlaylunel.html

std::string s = "hi";  s += "!";
来源：http://hz.nanxinkj.top/gtszyrcywu.html

[S33] C++：vector 增删
来源：http://hz.zhengqikj.top/gtvvxsduih.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.zhengqikj.top/gttlmotfdu.html

[S34] C++：遍历 vector
来源：http://hz.ivvv.top/gtxbfmadpc.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.xingfuxueyuan.xyz/gthzdlgcoo.html

[S35] C++：map
来源：http://hz.jqgfzy.top/gtpynoxvlg.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.snrcjt.cn/gtypmvanrd.html

[S36] C++：unordered_map
来源：http://hz.wangdashe.top/gtdwkbcoud.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zdqjudy.top/gtfibynods.html

[S37] C++：set
来源：http://hz.chenjidiqi.icu/gtyweuccth.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.havefunace.top/gtmzvhksqd.html

[S38] C++：排序
来源：http://hz.hongshengwenyu.top/gtbtqhgrhh.html

std::sort(v.begin(), v.end());
来源：http://hz.ydzc1.top/gtwezifnnr.html

[S39] C++：自定义比较器排序
来源：http://hz.jinqigufen.top/gtodlryrna.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.dashuyun.cn/gtvbiejcey.html

[S40] C++：查找元素
来源：http://hz.316326.xyz/gtzsokzsfk.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.ywan-chungtsiang.top/gtgwfvxukz.html

[S41] C++：类与构造函数
来源：http://hz.hammf.cn/gtlnwyntph.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.iojbl.cn/gtpxiistwt.html

[S42] C++：继承与虚函数
来源：http://hz.redwolf501.top/gtxpflgznh.html

class B : public Base { public: void f() override {} };
来源：http://hz.zhiwuduotai.top/gtqhvqryll.html

[S43] C++：智能指针
来源：http://hz.jqgufenzy.top/gtesjuiyru.html

auto p = std::make_unique<int>(5);
来源：http://hz.bjfxy.top/gtovpwurqo.html

[S44] C++：引用传参
来源：http://hz.pengpengdd.cyou/gtrelxenhw.html

void inc(int &x) { ++x; }
来源：http://hz.shuidangran.top/gtgrxqhplc.html

[S45] C++：lambda
来源：http://hz.ywan-chungtsiang.top/gtegwluzpg.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.ybcxt.top/gttbjqtror.html

[S46] C++：函数模板
来源：http://hz.birdmap.top/gteqiqfrpf.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.feifeiyinyue.top/gtydhkaiuo.html

[S47] C++：结构化绑定遍历
来源：http://hz.svipenyu.cn/gtlkebvrdy.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.nwbrower.top/gtiznqeyny.html

[S48] C++：逐行读文件
来源：http://hz.redwolf501.top/gtkrvsxrrm.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.zycfv.cn/gtkojuwtxr.html

while (std::getline(in, line)) { }
来源：http://hz.jinghuilouyu.cn/gtxjkswpys.html

[S49] C++：写文件
来源：http://hz.yuanzhike.top/gtfeegqdzu.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.jyoumei.cn/gthhwblvsx.html

[S50] C++：格式化数字
来源：http://hz.chenjidiqi.icu/gtyhgtfwga.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.shangyingyoupin.top/gtugomello.html

[S51] C++：显式类型转换
来源：http://hz.jqgfzy.top/gtkmfkalvu.html

static_cast<double>(a) / b
来源：http://hz.chenjidiqi.icu/gtweohblhq.html

[S52] C++：const 与 noexcept
来源：http://hz.cheryme.top/gtsibkmwda.html

int size() const noexcept { return n_; }
来源：http://hz.hywenlv.cn/gtiqgpstlr.html

[S53] C++：移动语义
来源：http://hz.shanyushiyangkeji.top/gtixjjobnu.html

std::vector<int> w = std::move(v);
来源：http://hz.svipenyu.cn/gtmzrjeblf.html

[S54] C++：异常处理
来源：http://hz.meibo888.top/gtcxluvrme.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.wangdashe.top/gtxclxsedg.html

[S55] C++：结构化绑定
来源：http://hz.tanke756.top/gthtxaautj.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.pengpengdd.cyou/gtxhtbiejb.html

[S56] C++：optional
来源：http://hz.hnqzz.top/gtkhqdfagc.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.feifeiyinyue.top/gtnmvnyjgn.html

[S57] C++：编译期常量
来源：http://hz.aibaodan.cn/gtwflymbsu.html

constexpr int N = 10;
来源：http://hz.hfpthk.cn/gttlfnqcll.html

[S58] C++：命名空间
来源：http://hz.hfpthk.cn/gtbyjhfojc.html

namespace ns { int f() { return 1; } }
来源：http://hz.yj20258.top/gtickpcxhk.html

[S59] C++：静态断言
来源：http://hz.hammf.cn/gtptlbqvwz.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.shangyingyoupin.top/gtpedsviku.html

[S60] C++：遍历并删除元素
来源：http://hz.havefunace.top/gtwzunrpxc.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.zhijiandao.cn/gtutocelzz.html

================================================================================
来源：http://hz.quarkkingdee.top/gtzgumogay.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.nanxuanxn.top/gtpmzcissl.html

================================================================================
来源：http://hz.jqgufenzy.top/gtodbekelz.html

[T01] Kotlin：Hello World
来源：http://hz.yangfankeji.com/gtrsmcxujf.html

println("Hello")
来源：http://hz.shanyushiyangtech.top/gtwzxvrwwz.html

[T02] Kotlin：变量
来源：http://hz.sufxvd.cn/gtkawktkyl.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.jlsjyb.cn/gtjuuwrzoi.html

[T03] Kotlin：字符串模板
来源：http://hz.iojbl.cn/gtvwevymdc.html

"值: $b"
来源：http://hz.hywenlv.cn/gtjjtqnezj.html

[T04] Kotlin：空安全
来源：http://hz.ivvv.top/gttcsqpjrq.html

val n: String? = null;  n?.length
来源：http://hz.zhengqikj.top/gtbemukodt.html

[T05] Kotlin：when 表达式
来源：http://hz.snrcjt.cn/gtblknoebc.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.guowangkeji.top/gtwbnduuyx.html

[T06] Kotlin：集合映射
来源：http://hz.jinyuanbaomall.cn/gtvarpggfd.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.daxiang520.top/gtjyeesafb.html

[T07] Kotlin：集合过滤
来源：http://hz.yj20258.top/gtfspdodud.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.tianlin.xyz/gtorftuubz.html

[T08] Kotlin：数据类
来源：http://hz.jinghuilouyu.cn/gtgeljzcxt.html

data class User(val name: String, val age: Int)
来源：http://hz.zhengqikj.top/gtogommhri.html

[T09] Kotlin：扩展函数
来源：http://hz.ppjwa.cn/gtutvezbmy.html

fun String.exclaim() = this + "!"
来源：http://hz.zhengqikj.top/gtxfbmqans.html

[T10] Kotlin：默认参数
来源：http://hz.cucudq.cn/gthudvjhvd.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.pengpengdd.cyou/gtohzzlxau.html

[T11] Kotlin：协程
来源：http://hz.yangfankeji.com/gtwsvdpbkc.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.quarkkingdee.top/gttxbtjnrs.html

[T12] Kotlin：解构声明
来源：http://hz.xziqi.cn/gtkuadffqc.html

val (a, b) = Pair(1, 2)
来源：http://hz.c1oappe.top/gtnvgvzrbb.html

[T13] Kotlin：只读 Map
来源：http://hz.zycfv.cn/gtrpugchqy.html

val m = mapOf("a" to 1)
来源：http://hz.ydjk.org.cn/gtmhmcnype.html

[T14] Kotlin：循环
来源：http://hz.yangfankeji.com/gtfmiafaji.html

for (i in 1..10) println(i)
来源：http://hz.xziqi.cn/gtzyuiegxh.html

[T15] Kotlin：接口
来源：http://hz.zhiwuduotai.top/gtpjyvtxzn.html

interface Shape { fun area(): Double }
来源：http://hz.yuanzhike.top/gtzjfhecfh.html

[T16] Swift：Hello World
来源：http://hz.birdmap.top/gtendkkufe.html

print("Hello")
来源：http://hz.zhongyouzk.top/gtvfedmgls.html


<!-- 参考信息 -->