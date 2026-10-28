代发 wailian999

[Q82] 字符长度与字节长度
来源：http://hz.tanke756.top/gtbjsuogwl.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.jqgufenzy.top/gtudzjsqde.html

[Q83] 大小写转换
来源：http://hz.shuidangran.top/gtsdqrgvvi.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.sweek.top/gtiyhnhwqj.html

[Q84] 去除首尾空格
来源：http://hz.guannengcc.top/gtxbaxihag.html

SELECT TRIM(name) FROM users;
来源：http://hz.wangshuangyany.cn/gtyyjxohsf.html

[Q85] 数值取整
来源：http://hz.jiagoushi.top/gtwyrfkeic.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.yvedp.cn/gtilefvgml.html

[Q86] 读取 JSON 字段
来源：http://hz.ybcxt.top/gtsnlheawi.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.hnxiangtu.top/gtuhanrwgi.html

[Q87] JSON 字段做条件
来源：http://hz.guowangkeji.top/gtpbhyzwyu.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.xuetiantiany.cn/gthtmivtck.html

[Q88] 行转列（条件聚合）
来源：http://hz.hnqzz.top/gtxmednnzl.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.feifeiyinyue.top/gtvvoadydw.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.nwbrower.top/gtrmjokaud.html

[Q89] 判断表是否存在
来源：http://hz.ydzc1.top/gtrailnocy.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.pycfn.com/gtpljlkjop.html

[Q90] 生成序号列
来源：http://hz.zhoulong.xyz/gtynbpokzr.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.yj202588.top/gtyaibbekl.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtgzriomjw.html

R. Bash 专题
来源：http://hz.ydjk.org.cn/gtkkagliku.html

================================================================================
来源：http://hz.sxryk.cn/gtbioklzhz.html

[R01] shebang 与严格模式
来源：http://hz.nanxinkj.top/gthzxxemiv.html

#!/usr/bin/env bash
来源：http://hz.daxiang520.top/gtrgsjatlb.html

set -euo pipefail
来源：http://hz.kuanghao11.cn/gtpceqkmmd.html

[R02] 变量赋值与使用
来源：http://hz.zhongyouzk.top/gtugtuiytc.html

name="Tom"; echo "$name"
来源：http://hz.tianlin.xyz/gtsdhxoshr.html

[R03] 只读变量
来源：http://hz.xuetiantiany.cn/gthqbbmfvf.html

readonly PI=3.14
来源：http://hz.yonumen.top/gtxcinllfi.html

[R04] 位置参数
来源：http://hz.jiagoushi.top/gtlslgjnka.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.mhx1999.top/gthsaqiwvz.html

[R05] 参数默认值
来源：http://hz.hongshengwenyu.top/gtcetehxcp.html

name="${1:-default}"
来源：http://hz.yj202588.top/gtulaguuoc.html

[R06] 判断命令是否存在
来源：http://hz.hysaishi.cn/gtfeawaamw.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.zdqjudy.top/gtnlegychw.html

[R07] if 判断文件
来源：http://hz.pycfn.com/gtoimimxod.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.sufxvd.cn/gtzsmwnhsu.html

[R08] 数值比较
来源：http://hz.jqgufenzy.top/gtortexbak.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.tian-w.cn/gtvenlpolz.html

[R09] 字符串比较
来源：http://hz.jinyuanbaomall.cn/gticpakptu.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.hnqzz.top/gtnsmuicrb.html

[R10] 正则匹配
来源：http://hz.316326.xyz/gtdzirvjoo.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.chenzaomai.com/gtivomvyxj.html

[R11] case 多分支
来源：http://hz.zycfv.cn/gtvchvcrjd.html

case "$1" in
来源：http://hz.xuanzx.com/gtnwyqnsjn.html

start) echo "启动" ;;
来源：http://hz.zhijiandao.cn/gtixjnljkp.html

stop)  echo "停止" ;;
来源：http://hz.jyoumei.cn/gtemmzekhp.html

*)     echo "未知命令" ;;
来源：http://hz.ivvv.top/gtneazqdxr.html

esac
来源：http://hz.ydjk.org.cn/gtwtnfqufs.html

[R12] for 遍历文件
来源：http://hz.shangyingyoupin.top/gtxiwhjxse.html

for f in *.txt; do echo "$f"; done
来源：http://hz.yvedp.cn/gtzmqjtbph.html

[R13] for 计数循环
来源：http://hz.cheryme.top/gthhmdldft.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.snrcjt.cn/gtospatmyj.html

[R14] C 风格 for
来源：http://hz.fengsongda.top/gtzjmnhgap.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.cdnleiting.top/gtmzahqvsb.html

[R15] while 逐行读文件
来源：http://hz.jinyuanbaomall.cn/gtfrcjjelk.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.shuidangran.top/gthbfsugbr.html

[R16] until 等待条件
来源：http://hz.haohaochexian.top/gtwbsdsraq.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.zhoulong.xyz/gtegliaqly.html

[R17] 数组定义与取值
来源：http://hz.svipenyu.cn/gteotuedug.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.chenlongwang.top/gtbiitmkgh.html

[R18] 遍历数组
来源：http://hz.ywan-chungtsiang.top/gtslezeown.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.xuanzx.com/gtsownjwcr.html

[R19] 数组长度
来源：http://hz.ybcxt.top/gtpvmalamg.html

echo "${#arr[@]}"
来源：http://hz.52xcode.cn/gtcwlomkep.html

[R20] 关联数组（字典）
来源：http://hz.shuidangran.top/gtfttcyuof.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.yongpay.top/gtikmfnlxk.html

[R21] 字符串长度
来源：http://hz.52xcode.cn/gtczqsuary.html

echo "${#s}"
来源：http://hz.0kj1m.cn/gtrkkesjan.html

[R22] 截取子串
来源：http://hz.iojbl.cn/gtreiwoquk.html

echo "${s:0:5}"
来源：http://hz.shuidangran.top/gtwxuhptfb.html

[R23] 字符串替换
来源：http://hz.jqgfzy.top/gtzruwjvdk.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.shanyushiyangkeji.top/gtbquvaiyi.html

[R24] 大小写转换
来源：http://hz.zhiwuduotai.top/gtkexntwqw.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.zhijiandao.cn/gtaqpbsfnv.html

[R25] 去后缀 / 去前缀
来源：http://hz.zycfv.cn/gtoglzyfxc.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.tianlin.xyz/gtzuerxswk.html

[R26] 命令替换
来源：http://hz.aibaodan.cn/gtcfflfdir.html

now=$(date +%F); echo "$now"
来源：http://hz.xuanzx.com/gtmvwqfxkv.html

[R27] 算术展开
来源：http://hz.pengpengdd.cyou/gtbrzmecsb.html

echo $((1 + 2 * 3))
来源：http://hz.ywan-chungtsiang.top/gtpycuwyar.html

[R28] 浮点运算
来源：http://hz.yj20258888.top/gttrgsexkz.html

echo "scale=2; 10/3" | bc
来源：http://hz.kuanghao11.cn/gtghzdtiei.html

[R29] 定义函数
来源：http://hz.hnxiangtu.top/gtccjyahqm.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.chenlongwang.top/gtmofchwwu.html

[R30] 函数返回状态码
来源：http://hz.xuanzx.com/gtmyshiyhi.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.yongpay.top/gtqzglqllq.html

[R31] 局部变量
来源：http://hz.shangyingyoupin.top/gtyytiqesh.html

f() { local x=1; echo "$x"; }
来源：http://hz.gaohongyu789.top/gtkldtaieb.html

[R32] 参数个数校验
来源：http://hz.dashuyun.cn/gtaghfzykw.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.zhiwuduotai.top/gtcrhhvdps.html

[R33] 捕获错误并提示行号
来源：http://hz.meibo888.top/gtvikohqmj.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.pycfn.com/gtuntcaecf.html

[R34] 退出时清理
来源：http://hz.zhongyouzk.top/gtkchqnqsx.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.hywenlv.cn/gtxopopgek.html

[R35] 后台执行并等待
来源：http://hz.fzhhl.top/gtugzuxvmy.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.52xcode.cn/gtoughxbob.html

[R36] 并发执行多个任务
来源：http://hz.sweek.top/gtghhjropq.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.fengsongda.top/gtaupmjvwu.html

[R37] 把输出赋给变量
来源：http://hz.wangshuangyany.cn/gtfdepngtm.html

files=$(ls -1)
来源：http://hz.jyoumei.cn/gtqpwioibc.html

[R38] 管道串联
来源：http://hz.sxryk.cn/gtckuzewle.html

cat a.txt | grep -i error | wc -l
来源：http://hz.smart0.xyz/gtryobltsb.html

[R39] 重定向标准输出与错误
来源：http://hz.zhengqikj.top/gtcwwylsic.html

cmd > out.log 2>&1
来源：http://hz.chenjidiqi.icu/gtaxpdummn.html

[R40] 追加写日志
来源：http://hz.jinqigfzy.top/gtupclmcsn.html

echo "log" >> out.log
来源：http://hz.yonumen.top/gtzjmmyfbb.html

[R41] 丢弃输出
来源：http://hz.yuxming.cn/gtuhdljhwd.html

cmd >/dev/null 2>&1
来源：http://hz.havefunace.top/gtbdxfcfzb.html

[R42] 输入重定向
来源：http://hz.feifeiyinyue.top/gtqhylhumy.html

wc -l < a.txt
来源：http://hz.smart0.xyz/gtjxlgtaow.html

[R43] 按名字查找文件
来源：http://hz.andypj.xyz/gtpgiwhkre.html

find . -name "*.log" -type f
来源：http://hz.gotoacloud.top/gtuvqpezjw.html

[R44] 按修改时间查找
来源：http://hz.nanxuanxn.top/gtzqmbfghx.html

find . -mtime -7 -type f
来源：http://hz.gogol.net.cn/gtiktgzmih.html

[R45] 批量删除
来源：http://hz.nanxuanxn.top/gtncdpaiap.html

find . -name "*.tmp" -delete
来源：http://hz.nanxuanxn.top/gtfucwwhtm.html

[R46] 递归替换文件内容
来源：http://hz.daria6918.cn/gtmovlckey.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.nwbrower.top/gtupmdjrwi.html

[R47] sed 单行替换
来源：http://hz.tian-w.cn/gtgqoiaaka.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.zhiwuduotai.top/gtjkcwhhpb.html

[R48] awk 取指定列
来源：http://hz.quarkkingdee.top/gthtgkagnq.html

awk '{print $1, $3}' a.txt
来源：http://hz.smart0.xyz/gtqvpriyzm.html

[R49] awk 带条件
来源：http://hz.daxiang520.top/gtncvfrsam.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.yuxming.cn/gtjeylcpmt.html

[R50] awk 求和
来源：http://hz.jyoumei.cn/gtaqfsebeq.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.yuanzhike.top/gtoatzguwh.html

[R51] 排序去重取前几
来源：http://hz.guowangkeji.top/gtdzxazxzg.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.fzhhl.top/gttdsvuhex.html

[R52] 统计行数
来源：http://hz.zhijiandao.cn/gtckhivlbb.html

wc -l a.txt
来源：http://hz.hysaishi.cn/gtsbkbettc.html

[R53] 查看文件头与实时尾
来源：http://hz.yangfankeji.com/gtynuohjji.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.hnxiangtu.top/gtiwsishde.html

[R54] 比较两个文件
来源：http://hz.zdqjudy.top/gtfnhvqrky.html

diff a.txt b.txt
来源：http://hz.yuanzhike.top/gtbaxauqiu.html

[R55] 压缩与解压
来源：http://hz.hywenlv.cn/gtltwdlxfz.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.daria6918.cn/gtovdjowzv.html

[R56] 远程拷贝
来源：http://hz.jianghu66.top/gtbvroadtx.html

scp file user@host:/path/
来源：http://hz.zhoulong.xyz/gtastlafey.html

[R57] 远程执行命令
来源：http://hz.jinyuanbaomall.cn/gtjpqupawz.html

ssh user@host 'uptime'
来源：http://hz.gaohongyu789.top/gtqlrcxsuo.html

[R58] 下载文件
来源：http://hz.shanyushiyangtech.top/gtrzubtekq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.pengpengdd.cyou/gtugwquyks.html

[R59] 发 POST JSON
来源：http://hz.yangfankeji.com/gteelykuln.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.xingfuxueyuan.xyz/gtrbwcjibd.html

[R60] 只看 HTTP 状态码
来源：http://hz.tanke756.top/gtpdwlfeat.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.hysaishi.cn/gtqleybdth.html

[R61] 磁盘占用
来源：http://hz.iojbl.cn/gtbgkjewnv.html

df -h;  du -sh *
来源：http://hz.xingfuxueyuan.xyz/gtfxtimnos.html

[R62] 找最占空间的文件
来源：http://hz.chenjidiqi.icu/gtzwcntbiq.html

du -ah . | sort -rh | head -10
来源：http://hz.feifeiyinyue.top/gtzqbzrant.html

[R63] 内存与进程
来源：http://hz.shuidangran.top/gtgjygpbch.html

free -h;  ps aux | grep nginx
来源：http://hz.ppjwa.cn/gtjxgvobcz.html

[R64] 结束进程
来源：http://hz.xuanzx.com/gthgrcikrq.html

kill -9 $(pgrep -f app.py)
来源：http://hz.havefunace.top/gtdjkxuzgn.html

[R65] 查看端口占用
来源：http://hz.aibaodan.cn/gtcnjthtpk.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.tianlin.xyz/gtgpplwadx.html

[R66] 定时任务
来源：http://hz.tanke756.top/gtrxxoyhnb.html

crontab -e;  crontab -l
来源：http://hz.jlsjyb.cn/gttzyjamno.html

[R67] 生成随机十六进制串
来源：http://hz.smart0.xyz/gtvatxoxtu.html

openssl rand -hex 16
来源：http://hz.zhoulong.xyz/gtaijvtfrf.html

[R68] 计算文件校验值
来源：http://hz.jqgufenzy.top/gtgwcbzwos.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.cucudq.cn/gttprfyzfd.html

[R69] 生成随机密码
来源：http://hz.9152youxi.cn/gtuuxflpsh.html

head -c 16 /dev/urandom | base64
来源：http://hz.yonumen.top/gtricbqjkf.html

[R70] 时间戳与互转
来源：http://hz.fengsongda.top/gthswldwuw.html

date +%s;  date -d @1700000000
来源：http://hz.gzhubu.top/gtvwopytgn.html

[R71] 日期格式化
来源：http://hz.tian-w.cn/gtgkzwbadp.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.jinghuilouyu.cn/gtlwpopgyt.html

[R72] 等待端口就绪
来源：http://hz.feifeiyinyue.top/gtptbxyutu.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.zdqjudy.top/gtkgjhiywt.html

[R73] 分割大日志
来源：http://hz.daria6918.cn/gthptdaafp.html

split -l 1000 big.log part_
来源：http://hz.hywenlv.cn/gtawawpuxt.html

[R74] 批量重命名
来源：http://hz.sufxvd.cn/gtyktdatxh.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.yvedp.cn/gtcjqxsqyg.html

[R75] 导出环境变量
来源：http://hz.meibo888.top/gtgtaoqfyr.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.zhaomingkeji.xyz/gtvptbrznv.html

[R76] 使用临时文件
来源：http://hz.cheryme.top/gtzipwetqq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.cdnleiting.top/gtyfcpqtph.html

[R77] 读取用户输入
来源：http://hz.hongshengwenyu.top/gtvyyceoji.html

read -rp "请输入: " ans
来源：http://hz.cucudq.cn/gtmxdtdyde.html

[R78] 交互式菜单
来源：http://hz.svipenyu.cn/gteqdqttzw.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.xinyue.icu/gtvvwjzexc.html

[R79] 解析命令行选项
来源：http://hz.jiagoushi.top/gtmyjxaxdn.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.iojbl.cn/gtkzwkjxow.html

[R80] 查看脚本执行耗时
来源：http://hz.bjfxy.top/gtojzwbvbh.html

time ./run.sh
来源：http://hz.316326.xyz/gtfpltkhtq.html

================================================================================
来源：http://hz.aizwys.cn/gtosphgmkh.html

S. C / C++ 专题
来源：http://hz.ywan-chungtsiang.top/gttjcemghk.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtkhtbyhtb.html

[S01] C：Hello World
来源：http://hz.guannengcc.top/gtjgxystfe.html

#include <stdio.h>
来源：http://hz.ivvv.top/gtjjqaqihr.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.dianchejie.cn/gtdmdnroun.html

[S02] C：变量与格式化输出
来源：http://hz.ybcxt.top/gtjekmkhps.html

int a = 10; printf("%d\n", a);
来源：http://hz.redwolf501.top/gtfwxnbjks.html

[S03] C：读入整数
来源：http://hz.havefunace.top/gtdonbsegy.html

int x; scanf("%d", &x);
来源：http://hz.vqdsnc.cn/gtstuykski.html

[S04] C：字符串复制
来源：http://hz.birdmap.top/gtamcrbxcp.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.zhengqikj.top/gtprbyglaz.html

[S05] C：字符串长度
来源：http://hz.xylfe.cn/gtrpslrlob.html

strlen(s)
来源：http://hz.yanxiufei.cn/gtriibsldi.html

[S06] C：字符串比较
来源：http://hz.ppjwa.cn/gtpwsyozyt.html

strcmp(a, b) == 0
来源：http://hz.gaohongyu789.top/gthxoapscd.html

[S07] C：数组遍历求和
来源：http://hz.52xcode.cn/gtoyxxsbex.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.haohaochexian.top/gtxgpefocj.html

[S08] C：动态内存分配与释放
来源：http://hz.ywan-chungtsiang.top/gtdrinptdd.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.nwbrower.top/gtndvkwjis.html

[S09] C：结构体定义与初始化
来源：http://hz.feifeiyinyue.top/gtzutxmhmb.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.bjfxy.top/gtpzkutnsa.html

[S10] C：指针与解引用
来源：http://hz.hongshengwenyu.top/gtyzcbxbfe.html

int *p = &a;  *p = 5;
来源：http://hz.jinqigufen.top/gtwagzrsgl.html

[S11] C：逐行读文件
来源：http://hz.yangfankeji.com/gtvbzcmofo.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.yj202588.top/gtqzalhatf.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.hysaishi.cn/gtxorhnsjh.html

fclose(f);
来源：http://hz.guannengcc.top/gtoxqytoie.html

[S12] C：写文件
来源：http://hz.52xcode.cn/gttzdntbiv.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.shangyingyoupin.top/gtonrwdvvn.html

[S13] C：宏定义
来源：http://hz.hnxiangtu.top/gtvxqfcmsa.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.cqqwz.cn/gtrzjwbiba.html

[S14] C：枚举
来源：http://hz.yangfankeji.com/gtdnwzqtiu.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.sysykeji.top/gtiektomhh.html

[S15] C：类型转换
来源：http://hz.daria6918.cn/gtovzmrevv.html

(double) a / b
来源：http://hz.yuanzhike.top/gtsicehtvt.html

[S16] C：位操作置位
来源：http://hz.tianlin.xyz/gtldpeotqv.html

x |= (1 << 3);
来源：http://hz.ivvv.top/gtkoqpesia.html

[S17] C：安全拼接字符串
来源：http://hz.nanxuanxn.top/gtbwxyzocj.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.zhijiandao.cn/gtiuvlbycu.html

[S18] C：命令行参数
来源：http://hz.chenzaomai.com/gtldiglats.html

int main(int argc, char **argv)
来源：http://hz.yj20258888.top/gtbgaewhpr.html

[S19] C：快速排序
来源：http://hz.jinqigufen.top/gtwegkwhmd.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.cashguo.top/gtqnsyktbx.html

[S20] C：二分查找
来源：http://hz.quarkkingdee.top/gtwgvlqptk.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.cashguo.top/gtfquvjqkh.html

[S21] C：字符类别判断
来源：http://hz.xuetiantiany.cn/gtrhkpqzty.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.jianghu66.top/gteogixclw.html

[S22] C：字符串转数字
来源：http://hz.xuetiantiany.cn/gtlpikeegw.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.bjfxy.top/gtfbdgtwzm.html

[S23] C：随机数
来源：http://hz.nwbrower.top/gtsjrhdcvq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.jinghuilouyu.cn/gtesieeqmy.html

[S24] C：获取本地时间
来源：http://hz.hnxiangtu.top/gtlrhxdhpg.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.ivvv.top/gtxgchfbqk.html

[S25] C：内存拷贝
来源：http://hz.jqgufenzy.top/gtoefgeehz.html

memcpy(dst, src, n);
来源：http://hz.hnxiangtu.top/gtpzqimbhq.html

[S26] C：内存清零
来源：http://hz.gogol.net.cn/gtkgtnrqwz.html

memset(a, 0, sizeof a);
来源：http://hz.ivvv.top/gtuyvfloyq.html

[S27] C：定义常量
来源：http://hz.dashuyun.cn/gtvjevdfyi.html

const double PI = 3.14159;
来源：http://hz.wangshuangyany.cn/gtwehemfaf.html

[S28] C：静态变量
来源：http://hz.zhixingplan.top/gtqypptdta.html

static int counter = 0;
来源：http://hz.bjfxy.top/gtszkbejfy.html

[S29] C：变参函数
来源：http://hz.zhengqikj.top/gtxhdoeyrv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.cqqwz.cn/gtwnqxsbpw.html

[S30] C：头文件保护
来源：http://hz.shangyingyoupin.top/gtacnifgti.html

#ifndef X_H
来源：http://hz.yj202588.top/gtmeysgtcv.html

#define X_H
来源：http://hz.ehwqpu.com/gtrccgwlfy.html

#endif
来源：http://hz.jinqigufen.top/gtuxomshli.html

[S31] C++：Hello World
来源：http://hz.cqqwz.cn/gtgpalvsye.html

#include <iostream>
来源：http://hz.ydjk.org.cn/gtkzxkearn.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.jqgufenzy.top/gtnivikqpc.html

[S32] C++：字符串
来源：http://hz.meibo888.top/gtsebgcgjn.html

std::string s = "hi";  s += "!";
来源：http://hz.c1oappe.top/gtiaxxgtax.html

[S33] C++：vector 增删
来源：http://hz.0kj1m.cn/gtmumyzaad.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.havefunace.top/gtyihtvjdm.html

[S34] C++：遍历 vector
来源：http://hz.feifeiyinyue.top/gtdhmmhdlf.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.hnxiangtu.top/gtqhchncrx.html

[S35] C++：map
来源：http://hz.hfpthk.cn/gtxkujrimf.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yj20258888.top/gtfkogfmkb.html

[S36] C++：unordered_map
来源：http://hz.hammf.cn/gtgibumrsp.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.tianlin.xyz/gtnljibehf.html

[S37] C++：set
来源：http://hz.shangyingyoupin.top/gtfoikzsez.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.xingfuxueyuan.xyz/gtbzjzzmfj.html

[S38] C++：排序
来源：http://hz.gogol.net.cn/gtkuvluclp.html

std::sort(v.begin(), v.end());
来源：http://hz.vqdsnc.cn/gtiegmgzkz.html

[S39] C++：自定义比较器排序
来源：http://hz.jinyuanbaomall.cn/gtakuhfnup.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.yanxiufei.cn/gtxfuhusto.html

[S40] C++：查找元素
来源：http://hz.xuanzx.com/gtygzdnwbe.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.nanxinkj.top/gtywyoxlsu.html

[S41] C++：类与构造函数
来源：http://hz.snrcjt.cn/gtffujvgsq.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.xuanzx.com/gtmaldhmrn.html

[S42] C++：继承与虚函数
来源：http://hz.316326.xyz/gttmclawdr.html

class B : public Base { public: void f() override {} };
来源：http://hz.wangshuangyany.cn/gttrsdifgx.html

[S43] C++：智能指针
来源：http://hz.jinyuanbaomall.cn/gthppmwdcu.html

auto p = std::make_unique<int>(5);
来源：http://hz.feifeiyinyue.top/gtrxnzkokp.html

[S44] C++：引用传参
来源：http://hz.havefunace.top/gtccsscahn.html

void inc(int &x) { ++x; }
来源：http://hz.jlsjyb.cn/gtnwhmbzuk.html

[S45] C++：lambda
来源：http://hz.aibaodan.cn/gtmlwcflpb.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.chenzaomai.com/gtvhnxntii.html

[S46] C++：函数模板
来源：http://hz.dashuyun.cn/gtdkjygmob.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.hnqzz.top/gtvaxhnjji.html

[S47] C++：结构化绑定遍历
来源：http://hz.xuetiantiany.cn/gtukbhoskm.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.jqgufenzy.top/gtxysiofwt.html

[S48] C++：逐行读文件
来源：http://hz.kuanghao11.cn/gtwfaarvjc.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.sweek.top/gtnhjibdbz.html

while (std::getline(in, line)) { }
来源：http://hz.hnqzz.top/gtnqlstkki.html

[S49] C++：写文件
来源：http://hz.svipenyu.cn/gtcrdaebwz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.yuxming.cn/gtracoohqn.html

[S50] C++：格式化数字
来源：http://hz.yangfankeji.com/gtquxrfmdj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.bjfxy.top/gtxytmajkh.html

[S51] C++：显式类型转换
来源：http://hz.jyoumei.cn/gtyxvhhjcf.html

static_cast<double>(a) / b
来源：http://hz.snrcjt.cn/gtogumwtbd.html

[S52] C++：const 与 noexcept
来源：http://hz.cheryme.top/gtxeibolne.html


<!-- 参考信息 -->