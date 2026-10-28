代发 wailian999

[Q80] 字符串截取
来源：http://hz.zhiwuduotai.top/gtsjolitvv.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.jinghuilouyu.cn/gtplpvrxkc.html

[Q81] 字符串替换
来源：http://hz.yj20258888.top/gtfgiexebl.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.quarkkingdee.top/gtpsolwhev.html

[Q82] 字符长度与字节长度
来源：http://hz.xylfe.cn/gtpcakfich.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.shanyushiyangtech.top/gtxcwsvlpx.html

[Q83] 大小写转换
来源：http://hz.ybcxt.top/gtlhpdivub.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.c1oappe.top/gtvhkxyfxe.html

[Q84] 去除首尾空格
来源：http://hz.dashuyun.cn/gtpclymquf.html

SELECT TRIM(name) FROM users;
来源：http://hz.sxryk.cn/gtwjwduqxt.html

[Q85] 数值取整
来源：http://hz.9152youxi.cn/gtrtowjqdn.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.yueranfly.top/gtwqscsiij.html

[Q86] 读取 JSON 字段
来源：http://hz.haohaochexian.top/gtbjgdvivq.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.ehwqpu.com/gtlggaebgw.html

[Q87] JSON 字段做条件
来源：http://hz.yj20258.top/gtomaknwep.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.xinyue.icu/gtrpjoydgi.html

[Q88] 行转列（条件聚合）
来源：http://hz.mhx1999.top/gtturhsvdi.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.tian-w.cn/gtmyeydwaz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.jinghuilouyu.cn/gtgmuwvshe.html

[Q89] 判断表是否存在
来源：http://hz.xuetiantiany.cn/gtcmqpugvf.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.kuanghao11.cn/gtodptedzz.html

[Q90] 生成序号列
来源：http://hz.guowangkeji.top/gtlbecmnhj.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.svipenyu.cn/gtyljrgufr.html

================================================================================
来源：http://hz.kuanghao11.cn/gtmlbmduqg.html

R. Bash 专题
来源：http://hz.sweek.top/gtgjhnalec.html

================================================================================
来源：http://hz.wangdashe.top/gtrbpupxdw.html

[R01] shebang 与严格模式
来源：http://hz.nwbrower.top/gtfsiwetkw.html

#!/usr/bin/env bash
来源：http://hz.chenlongwang.top/gtcrkdlagf.html

set -euo pipefail
来源：http://hz.kuanghao11.cn/gtebcizpdm.html

[R02] 变量赋值与使用
来源：http://hz.hnqzz.top/gtdfiunbqh.html

name="Tom"; echo "$name"
来源：http://hz.zhijiandao.cn/gtxyklcoqs.html

[R03] 只读变量
来源：http://hz.xuanzx.com/gtfwftxulc.html

readonly PI=3.14
来源：http://hz.yj20258.top/gtzyoyydiy.html

[R04] 位置参数
来源：http://hz.chenlongwang.top/gtkbtrbfld.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.ehwqpu.com/gtyefuwpkp.html

[R05] 参数默认值
来源：http://hz.nanxuanxn.top/gtaqkylthd.html

name="${1:-default}"
来源：http://hz.dianchejie.cn/gtotzyfibu.html

[R06] 判断命令是否存在
来源：http://hz.ydzc1.top/gtimxracbu.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.hywenlv.cn/gtwhqyqbha.html

[R07] if 判断文件
来源：http://hz.pengpengdd.cyou/gtqjtzgxnn.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.sysykeji.top/gtmjiynbah.html

[R08] 数值比较
来源：http://hz.cashguo.top/gtdcxjpcoo.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.ehwqpu.com/gtiotirfgm.html

[R09] 字符串比较
来源：http://hz.ywan-chungtsiang.top/gthwvdgbdm.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.xylfe.cn/gtgrxraomj.html

[R10] 正则匹配
来源：http://hz.yueranfly.top/gtohdudvgn.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.redwolf501.top/gtcvntxwjz.html

[R11] case 多分支
来源：http://hz.316326.xyz/gtotspvasv.html

case "$1" in
来源：http://hz.dashuyun.cn/gtfsclpfvn.html

start) echo "启动" ;;
来源：http://hz.aibaodan.cn/gtputabfer.html

stop)  echo "停止" ;;
来源：http://hz.52xcode.cn/gtqytfddhk.html

*)     echo "未知命令" ;;
来源：http://hz.feifeiyinyue.top/gtvhxxnpyp.html

esac
来源：http://hz.cqqwz.cn/gtpprqzsli.html

[R12] for 遍历文件
来源：http://hz.52xcode.cn/gtmoncqeuc.html

for f in *.txt; do echo "$f"; done
来源：http://hz.dianchejie.cn/gtolbjnysh.html

[R13] for 计数循环
来源：http://hz.daxiang520.top/gtsxqseaer.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.ehwqpu.com/gtoqdnbbgw.html

[R14] C 风格 for
来源：http://hz.daria6918.cn/gtczinatfs.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.xylfe.cn/gtctqswgjb.html

[R15] while 逐行读文件
来源：http://hz.yangfankeji.com/gtgxrevyxc.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.cheryme.top/gtjzceprzb.html

[R16] until 等待条件
来源：http://hz.hammf.cn/gtqpotqicz.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.ydzc1.top/gtnoqljshi.html

[R17] 数组定义与取值
来源：http://hz.snrcjt.cn/gtzbdqthfd.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.hfpthk.cn/gttqthyeos.html

[R18] 遍历数组
来源：http://hz.tanke756.top/gtckwsvysh.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.zdqjudy.top/gtqlgrdylh.html

[R19] 数组长度
来源：http://hz.xinyue.icu/gtxfjcgzzt.html

echo "${#arr[@]}"
来源：http://hz.shzxlz.cn/gtwzlwmchi.html

[R20] 关联数组（字典）
来源：http://hz.cashguo.top/gtsfkrrvvp.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.jianghu66.top/gtpzwlhsbm.html

[R21] 字符串长度
来源：http://hz.tanke756.top/gtpdfcutag.html

echo "${#s}"
来源：http://hz.jianghu66.top/gtchiqkwov.html

[R22] 截取子串
来源：http://hz.zhongyouzk.top/gtlboxlhfp.html

echo "${s:0:5}"
来源：http://hz.xuanzx.com/gtijrkbguh.html

[R23] 字符串替换
来源：http://hz.shzxlz.cn/gtamzfpkfd.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.jyoumei.cn/gtzpinqinr.html

[R24] 大小写转换
来源：http://hz.vqdsnc.cn/gtwpbgnxzm.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.hfpthk.cn/gtbihgbssz.html

[R25] 去后缀 / 去前缀
来源：http://hz.tanke756.top/gtpywmeass.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.jinghuilouyu.cn/gtpxozyamd.html

[R26] 命令替换
来源：http://hz.tian-w.cn/gtujzlbgym.html

now=$(date +%F); echo "$now"
来源：http://hz.gaohongyu789.top/gtdkcmzlsn.html

[R27] 算术展开
来源：http://hz.ywan-chungtsiang.top/gtyutewhsi.html

echo $((1 + 2 * 3))
来源：http://hz.yongpay.top/gtyshtzzrw.html

[R28] 浮点运算
来源：http://hz.quarkkingdee.top/gtdnhhfaho.html

echo "scale=2; 10/3" | bc
来源：http://hz.ydjk.org.cn/gtbbzfzfpz.html

[R29] 定义函数
来源：http://hz.chenzaomai.com/gtajrvrrre.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.yangfankeji.com/gtmxedzsfb.html

[R30] 函数返回状态码
来源：http://hz.c1oappe.top/gtlnjqwhap.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.cheryme.top/gtwcbepiny.html

[R31] 局部变量
来源：http://hz.zhoulong.xyz/gtwmhqzqar.html

f() { local x=1; echo "$x"; }
来源：http://hz.316326.xyz/gtrugvexra.html

[R32] 参数个数校验
来源：http://hz.pycfn.com/gtbtgovfss.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.pengpengdd.cyou/gtmcrqkveu.html

[R33] 捕获错误并提示行号
来源：http://hz.daxiang520.top/gtsqpsjeln.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.zhengqikj.top/gtpsztnvjz.html

[R34] 退出时清理
来源：http://hz.vqdsnc.cn/gtogbxkcoh.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.hywenlv.cn/gtcuaxmuuj.html

[R35] 后台执行并等待
来源：http://hz.jianghu66.top/gtiacvmrso.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.dashuyun.cn/gtdlnipety.html

[R36] 并发执行多个任务
来源：http://hz.yj20258.top/gtodybomwc.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.yonumen.top/gtviufvxuv.html

[R37] 把输出赋给变量
来源：http://hz.hnxiangtu.top/gtwfpqvikl.html

files=$(ls -1)
来源：http://hz.fzhhl.top/gtjpvrspxb.html

[R38] 管道串联
来源：http://hz.iojbl.cn/gtngjdgnlz.html

cat a.txt | grep -i error | wc -l
来源：http://hz.yanxiufei.cn/gtxnvxmrcb.html

[R39] 重定向标准输出与错误
来源：http://hz.smart0.xyz/gtqvcmqbgw.html

cmd > out.log 2>&1
来源：http://hz.jinqigfzy.top/gtwfriyvqr.html

[R40] 追加写日志
来源：http://hz.hnxiangtu.top/gtdveuydlj.html

echo "log" >> out.log
来源：http://hz.daxiang520.top/gtuvfukuot.html

[R41] 丢弃输出
来源：http://hz.chenzaomai.com/gtrpccqjjl.html

cmd >/dev/null 2>&1
来源：http://hz.ehwqpu.com/gtxitglxfb.html

[R42] 输入重定向
来源：http://hz.hfpthk.cn/gtqqdkjdgy.html

wc -l < a.txt
来源：http://hz.zhaomingkeji.xyz/gtailfqhxh.html

[R43] 按名字查找文件
来源：http://hz.gogol.net.cn/gtdvviniuf.html

find . -name "*.log" -type f
来源：http://hz.quarkkingdee.top/gtsquhveoi.html

[R44] 按修改时间查找
来源：http://hz.wangshuangyany.cn/gttymfdqkv.html

find . -mtime -7 -type f
来源：http://hz.ivvv.top/gtgrffsxda.html

[R45] 批量删除
来源：http://hz.quarkkingdee.top/gthkxqiknt.html

find . -name "*.tmp" -delete
来源：http://hz.ivvv.top/gtynotfkxd.html

[R46] 递归替换文件内容
来源：http://hz.tanke756.top/gtsatnngmz.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.xinyue.icu/gtwneffbap.html

[R47] sed 单行替换
来源：http://hz.daxiang520.top/gtbnguloxp.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.wangdashe.top/gtevnncoas.html

[R48] awk 取指定列
来源：http://hz.bjfxy.top/gtrdboatei.html

awk '{print $1, $3}' a.txt
来源：http://hz.smart0.xyz/gttqvifwja.html

[R49] awk 带条件
来源：http://hz.xuetiantiany.cn/gtwezpooeo.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.yj202588.top/gtnufoznbu.html

[R50] awk 求和
来源：http://hz.jiagoushi.top/gtuhpsiaqw.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.yj20258888.top/gtdtwcqhws.html

[R51] 排序去重取前几
来源：http://hz.tian-w.cn/gtqrgmagvd.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.bjfxy.top/gtndcrmqri.html

[R52] 统计行数
来源：http://hz.52xcode.cn/gtzfqqxsqa.html

wc -l a.txt
来源：http://hz.hfpthk.cn/gtmmsnglal.html

[R53] 查看文件头与实时尾
来源：http://hz.smart0.xyz/gtpjjuzmss.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.nanxuanxn.top/gtpyqaoddz.html

[R54] 比较两个文件
来源：http://hz.zhengqikj.top/gthndpzwqy.html

diff a.txt b.txt
来源：http://hz.yvedp.cn/gtrzhhxhrq.html

[R55] 压缩与解压
来源：http://hz.dashuyun.cn/gtacntdfla.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.ybcxt.top/gtrdyvevol.html

[R56] 远程拷贝
来源：http://hz.havefunace.top/gtwjvjbrkm.html

scp file user@host:/path/
来源：http://hz.andypj.xyz/gtkuzgfwpc.html

[R57] 远程执行命令
来源：http://hz.zdqjudy.top/gtbbcomews.html

ssh user@host 'uptime'
来源：http://hz.zhixingplan.top/gtqwjimaol.html

[R58] 下载文件
来源：http://hz.chenjidiqi.icu/gtquwghbjo.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.316326.xyz/gtxdghhyyd.html

[R59] 发 POST JSON
来源：http://hz.fengsongda.top/gttykztmno.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.zhaomingkeji.xyz/gtudjcnlhc.html

[R60] 只看 HTTP 状态码
来源：http://hz.hammf.cn/gtvdrvrrkk.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.snrcjt.cn/gtihjvcfmn.html

[R61] 磁盘占用
来源：http://hz.zhongyouzk.top/gteixfvzer.html

df -h;  du -sh *
来源：http://hz.feifeiyinyue.top/gtcokunqje.html

[R62] 找最占空间的文件
来源：http://hz.daria6918.cn/gtzwncwxvw.html

du -ah . | sort -rh | head -10
来源：http://hz.svipenyu.cn/gtruyzhmuj.html

[R63] 内存与进程
来源：http://hz.xuetiantiany.cn/gtydxobzer.html

free -h;  ps aux | grep nginx
来源：http://hz.hongshengwenyu.top/gtpnicjksu.html

[R64] 结束进程
来源：http://hz.jiagoushi.top/gtvhxmbusz.html

kill -9 $(pgrep -f app.py)
来源：http://hz.hammf.cn/gtaiuicglz.html

[R65] 查看端口占用
来源：http://hz.yj20258.top/gtqlkzblll.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.aibaodan.cn/gtigyriqey.html

[R66] 定时任务
来源：http://hz.gzhubu.top/gtheempusr.html

crontab -e;  crontab -l
来源：http://hz.hfpthk.cn/gtynewjdkg.html

[R67] 生成随机十六进制串
来源：http://hz.vqdsnc.cn/gtphnwacee.html

openssl rand -hex 16
来源：http://hz.xuetiantiany.cn/gtbaqlmjjg.html

[R68] 计算文件校验值
来源：http://hz.kuanghao11.cn/gtybqixedz.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.9152youxi.cn/gtfdtdcrnw.html

[R69] 生成随机密码
来源：http://hz.shuidangran.top/gtweaodspi.html

head -c 16 /dev/urandom | base64
来源：http://hz.sxryk.cn/gtnxduwzin.html

[R70] 时间戳与互转
来源：http://hz.xuetiantiany.cn/gtkmbugclf.html

date +%s;  date -d @1700000000
来源：http://hz.yj202588.top/gtxuwjkhqz.html

[R71] 日期格式化
来源：http://hz.gogol.net.cn/gtyqwjrcag.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.zhengqikj.top/gtghlpdnbu.html

[R72] 等待端口就绪
来源：http://hz.gotoacloud.top/gtvuyzdoux.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.dashuyun.cn/gtrndxoqja.html

[R73] 分割大日志
来源：http://hz.cashguo.top/gtsuakqpil.html

split -l 1000 big.log part_
来源：http://hz.shanyushiyangtech.top/gtxxkczcah.html

[R74] 批量重命名
来源：http://hz.sysykeji.top/gtdvsnwhaw.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.tanke756.top/gtnogcschn.html

[R75] 导出环境变量
来源：http://hz.feifeiyinyue.top/gtqkwihncq.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.andypj.xyz/gtjxaahidn.html

[R76] 使用临时文件
来源：http://hz.yonumen.top/gtwdrozgsy.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.birdmap.top/gtckykkmqn.html

[R77] 读取用户输入
来源：http://hz.quarkkingdee.top/gtuyiuczcj.html

read -rp "请输入: " ans
来源：http://hz.chenzaomai.com/gtroexdoef.html

[R78] 交互式菜单
来源：http://hz.yj20258.top/gtvuhvxpid.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.chenlongwang.top/gtahazskuw.html

[R79] 解析命令行选项
来源：http://hz.daxiang520.top/gtdfcmnmke.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.yonumen.top/gthshvgdzo.html

[R80] 查看脚本执行耗时
来源：http://hz.cdnleiting.top/gtkcwkaqpu.html

time ./run.sh
来源：http://hz.haohaochexian.top/gtvgmodzdf.html

================================================================================
来源：http://hz.cashguo.top/gtsoqjdrtd.html

S. C / C++ 专题
来源：http://hz.daxiang520.top/gtsrskolsm.html

================================================================================
来源：http://hz.316326.xyz/gtruphubgz.html

[S01] C：Hello World
来源：http://hz.jyoumei.cn/gtvwjooktl.html

#include <stdio.h>
来源：http://hz.yueranfly.top/gtzcdovxtg.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.nanxinkj.top/gtyoqfienl.html

[S02] C：变量与格式化输出
来源：http://hz.zhongyouzk.top/gtrnlgcujf.html

int a = 10; printf("%d\n", a);
来源：http://hz.quarkkingdee.top/gtiknvckek.html

[S03] C：读入整数
来源：http://hz.aibaodan.cn/gtaogkfrjb.html

int x; scanf("%d", &x);
来源：http://hz.aibaodan.cn/gtgoqijomj.html

[S04] C：字符串复制
来源：http://hz.guowangkeji.top/gtvgfdlasl.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.jinghuilouyu.cn/gtvvgckeco.html

[S05] C：字符串长度
来源：http://hz.zhiwuduotai.top/gtezgwujcu.html

strlen(s)
来源：http://hz.hammf.cn/gtgaugfltt.html

[S06] C：字符串比较
来源：http://hz.yuxming.cn/gtmatbgvdv.html

strcmp(a, b) == 0
来源：http://hz.ywan-chungtsiang.top/gtcdvuxvze.html

[S07] C：数组遍历求和
来源：http://hz.jinyuanbaomall.cn/gtkmidznbk.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.haohaochexian.top/gtallgbprb.html

[S08] C：动态内存分配与释放
来源：http://hz.cqqwz.cn/gtgfqrkqdp.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.yonumen.top/gtmelnrfzt.html

[S09] C：结构体定义与初始化
来源：http://hz.9152youxi.cn/gtlrjctaow.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.ehwqpu.com/gtuzmbyior.html

[S10] C：指针与解引用
来源：http://hz.kuanghao11.cn/gtjpznpvtm.html

int *p = &a;  *p = 5;
来源：http://hz.ivvv.top/gtbuysydcu.html

[S11] C：逐行读文件
来源：http://hz.zhiwuduotai.top/gtvpjitixd.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.zhixingplan.top/gtxrhfpaca.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.cashguo.top/gtzunlnomd.html

fclose(f);
来源：http://hz.xuanzx.com/gtrnwjezqt.html

[S12] C：写文件
来源：http://hz.316326.xyz/gtxdbtlmjt.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.xuetiantiany.cn/gtlprkejsb.html

[S13] C：宏定义
来源：http://hz.jiagoushi.top/gtiifuvoii.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.jqgufenzy.top/gtmqlgwpki.html

[S14] C：枚举
来源：http://hz.redwolf501.top/gtocsiwrmz.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.mhx1999.top/gtcllxmlzp.html

[S15] C：类型转换
来源：http://hz.gotoacloud.top/gtfrwbwerx.html

(double) a / b
来源：http://hz.hongshengwenyu.top/gtmbzmukut.html

[S16] C：位操作置位
来源：http://hz.vqdsnc.cn/gtqddhifos.html

x |= (1 << 3);
来源：http://hz.aibaodan.cn/gtamlipjxp.html

[S17] C：安全拼接字符串
来源：http://hz.316326.xyz/gtovfkexwr.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.yuxming.cn/gtdryxnxql.html

[S18] C：命令行参数
来源：http://hz.xuanzx.com/gtnowekmta.html

int main(int argc, char **argv)
来源：http://hz.jianghu66.top/gtsvuwebok.html

[S19] C：快速排序
来源：http://hz.yuanzhike.top/gttwnifcqg.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.yvedp.cn/gtamjfraoe.html

[S20] C：二分查找
来源：http://hz.jlsjyb.cn/gtzoigtasu.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.yvedp.cn/gtwqfknxmb.html

[S21] C：字符类别判断
来源：http://hz.bjfxy.top/gtgnijhjwo.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.ydzc1.top/gtvloflnag.html

[S22] C：字符串转数字
来源：http://hz.zdqjudy.top/gtujbmkfrk.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.ehwqpu.com/gtasmtbtyt.html

[S23] C：随机数
来源：http://hz.yongpay.top/gtodbybghz.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.jqgfzy.top/gtejufdbgv.html

[S24] C：获取本地时间
来源：http://hz.xziqi.cn/gtcsqxugue.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.zhengqikj.top/gtkaevuqrr.html

[S25] C：内存拷贝
来源：http://hz.tianlin.xyz/gtxcesmbjo.html

memcpy(dst, src, n);
来源：http://hz.fzhhl.top/gtkiyjcugd.html

[S26] C：内存清零
来源：http://hz.0kj1m.cn/gtzqjubbdl.html

memset(a, 0, sizeof a);
来源：http://hz.nanxinkj.top/gtyhjcixol.html

[S27] C：定义常量
来源：http://hz.ybcxt.top/gthsrpyouh.html

const double PI = 3.14159;
来源：http://hz.aizwys.cn/gtdodyvwlq.html

[S28] C：静态变量
来源：http://hz.gaohongyu789.top/gtdqgqiqfg.html

static int counter = 0;
来源：http://hz.sysykeji.top/gtlxlbptku.html

[S29] C：变参函数
来源：http://hz.nanxinkj.top/gtrmwuxtij.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.xinyue.icu/gtklkmflti.html

[S30] C：头文件保护
来源：http://hz.dianchejie.cn/gtvidntwhr.html

#ifndef X_H
来源：http://hz.dianchejie.cn/gtwgvgwnoo.html

#define X_H
来源：http://hz.yj20258888.top/gthauuhgcp.html

#endif
来源：http://hz.316326.xyz/gtcgqdowmv.html

[S31] C++：Hello World
来源：http://hz.zhixingplan.top/gtrczthxsj.html

#include <iostream>
来源：http://hz.birdmap.top/gtnkotfwhu.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.birdmap.top/gtocdkhlaj.html

[S32] C++：字符串
来源：http://hz.tianlin.xyz/gtgzyjxsuh.html

std::string s = "hi";  s += "!";
来源：http://hz.yueranfly.top/gtbiwtcqfl.html

[S33] C++：vector 增删
来源：http://hz.aizwys.cn/gtkhtmnmcy.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.wangshuangyany.cn/gtriuudaht.html

[S34] C++：遍历 vector
来源：http://hz.hammf.cn/gtrmtvljzq.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.zhoulong.xyz/gtoxdecqhw.html

[S35] C++：map
来源：http://hz.zhixingplan.top/gtsnaruyiq.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.ivvv.top/gtcmexryvn.html

[S36] C++：unordered_map
来源：http://hz.iojbl.cn/gtpxnqdfaw.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.ydzc1.top/gtuyaapcip.html

[S37] C++：set
来源：http://hz.hysaishi.cn/gtjmkecfgr.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.pycfn.com/gtvxrhkjbw.html

[S38] C++：排序
来源：http://hz.meibo888.top/gtuoeufroe.html

std::sort(v.begin(), v.end());
来源：http://hz.jinqigufen.top/gttjniauoc.html

[S39] C++：自定义比较器排序
来源：http://hz.yangfankeji.com/gtjrwjjehd.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.smart0.xyz/gtwadbssjv.html

[S40] C++：查找元素
来源：http://hz.guowangkeji.top/gtbfcbnqfw.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.andypj.xyz/gtscbioxul.html

[S41] C++：类与构造函数
来源：http://hz.316326.xyz/gtzpgxmtbw.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.0kj1m.cn/gtcrhrybcg.html

[S42] C++：继承与虚函数
来源：http://hz.yongpay.top/gtvrddeguv.html

class B : public Base { public: void f() override {} };
来源：http://hz.svipenyu.cn/gtxsszoxpy.html

[S43] C++：智能指针
来源：http://hz.shangyingyoupin.top/gtyjoujlnu.html

auto p = std::make_unique<int>(5);
来源：http://hz.havefunace.top/gtswgncsxs.html

[S44] C++：引用传参
来源：http://hz.guowangkeji.top/gtwweajykm.html

void inc(int &x) { ++x; }
来源：http://hz.aizwys.cn/gtqptiknes.html

[S45] C++：lambda
来源：http://hz.yj202588.top/gtoaeroxpy.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.cucudq.cn/gtpskgdxdt.html

[S46] C++：函数模板
来源：http://hz.jqgfzy.top/gtbiiozpod.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.gotoacloud.top/gtrqnzaurt.html

[S47] C++：结构化绑定遍历
来源：http://hz.daria6918.cn/gtkbgdgjfc.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.ehwqpu.com/gthbjdbdld.html

[S48] C++：逐行读文件
来源：http://hz.dashuyun.cn/gttdhulnqv.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.hfpthk.cn/gtwqhwlnsa.html

while (std::getline(in, line)) { }
来源：http://hz.hongshengwenyu.top/gtvomqacbo.html

[S49] C++：写文件
来源：http://hz.xinyue.icu/gtoffscemn.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.cheryme.top/gtsxtsbwer.html

[S50] C++：格式化数字
来源：http://hz.sweek.top/gtfgbvmcwu.html


<!-- 参考信息 -->