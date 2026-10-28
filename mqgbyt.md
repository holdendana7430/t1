代发 wailian999

[Q76] 按天统计
来源：http://hz.ehwqpu.com/gtzyfqluot.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.ywan-chungtsiang.top/gtmbmwbubn.html

[Q77] 时间加减
来源：http://hz.ppjwa.cn/gtpdqxvrjp.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.yvedp.cn/gtransboil.html

[Q78] 当前时间
来源：http://hz.sufxvd.cn/gttjilwqtv.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.zhijiandao.cn/gtvxsnqgan.html

[Q79] 字符串拼接
来源：http://hz.smart0.xyz/gtunbttunv.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.zhixingplan.top/gtedufvlrj.html

[Q80] 字符串截取
来源：http://hz.shuidangran.top/gtvljqmcqd.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.jqgfzy.top/gtcezyqbdk.html

[Q81] 字符串替换
来源：http://hz.sufxvd.cn/gtijthsvbx.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.ehwqpu.com/gtinrqhsiw.html

[Q82] 字符长度与字节长度
来源：http://hz.shzxlz.cn/gtcfixhuhc.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.iojbl.cn/gtqofpkcdg.html

[Q83] 大小写转换
来源：http://hz.ydzc1.top/gtywqmgoks.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.tanke756.top/gtlsccpndb.html

[Q84] 去除首尾空格
来源：http://hz.zdqjudy.top/gttcfkormx.html

SELECT TRIM(name) FROM users;
来源：http://hz.zhongyouzk.top/gtkfmdxhtd.html

[Q85] 数值取整
来源：http://hz.zhoulong.xyz/gtnulcimmx.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.xingfuxueyuan.xyz/gtlsjschnn.html

[Q86] 读取 JSON 字段
来源：http://hz.wangshuangyany.cn/gtkwfzlmri.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.ywan-chungtsiang.top/gtxlvxgydi.html

[Q87] JSON 字段做条件
来源：http://hz.guowangkeji.top/gthayzxqyy.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.xylfe.cn/gtqdldrxcz.html

[Q88] 行转列（条件聚合）
来源：http://hz.zhoulong.xyz/gtipmgmaac.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.ybcxt.top/gtoitiajxp.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.xylfe.cn/gtlltpwnwt.html

[Q89] 判断表是否存在
来源：http://hz.redwolf501.top/gtikwzukih.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.shanyushiyangkeji.top/gtilkkzlpd.html

[Q90] 生成序号列
来源：http://hz.jqgufenzy.top/gtfgxciyhd.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.guannengcc.top/gtudipuxtn.html

================================================================================
来源：http://hz.smart0.xyz/gtfrinlbpx.html

R. Bash 专题
来源：http://hz.smart0.xyz/gtcekjtdwx.html

================================================================================
来源：http://hz.chenzaomai.com/gtmtbywsdu.html

[R01] shebang 与严格模式
来源：http://hz.jiagoushi.top/gttihdncwt.html

#!/usr/bin/env bash
来源：http://hz.hysaishi.cn/gtpykqhqhi.html

set -euo pipefail
来源：http://hz.gotoacloud.top/gtjqdzhjbo.html

[R02] 变量赋值与使用
来源：http://hz.xingfuxueyuan.xyz/gtujevpvxs.html

name="Tom"; echo "$name"
来源：http://hz.pycfn.com/gtturmiohz.html

[R03] 只读变量
来源：http://hz.c1oappe.top/gtfnqlyfqn.html

readonly PI=3.14
来源：http://hz.snrcjt.cn/gtilclxvhj.html

[R04] 位置参数
来源：http://hz.quarkkingdee.top/gthurvwpkd.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.jinqigufen.top/gtsodkhxiv.html

[R05] 参数默认值
来源：http://hz.snrcjt.cn/gtmembidoz.html

name="${1:-default}"
来源：http://hz.aizwys.cn/gtuvemoebn.html

[R06] 判断命令是否存在
来源：http://hz.shanyushiyangkeji.top/gtiwndsquh.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.zhoulong.xyz/gtnopnztze.html

[R07] if 判断文件
来源：http://hz.zhijiandao.cn/gtgjhnksmj.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.sxryk.cn/gtckdfpigg.html

[R08] 数值比较
来源：http://hz.zycfv.cn/gtyjnboqeh.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.c1oappe.top/gtrgmlhjmc.html

[R09] 字符串比较
来源：http://hz.jinqigufen.top/gtxviavioy.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.xziqi.cn/gteotyuexq.html

[R10] 正则匹配
来源：http://hz.gotoacloud.top/gthmagfmog.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.hammf.cn/gtfewmvkfe.html

[R11] case 多分支
来源：http://hz.jinqigfzy.top/gtbqzenxpa.html

case "$1" in
来源：http://hz.kuanghao11.cn/gtwpfyzzpw.html

start) echo "启动" ;;
来源：http://hz.yj20258888.top/gtbvcopmaw.html

stop)  echo "停止" ;;
来源：http://hz.ybcxt.top/gtoidwjenz.html

*)     echo "未知命令" ;;
来源：http://hz.gotoacloud.top/gttuqrcqse.html

esac
来源：http://hz.yuxming.cn/gtjnefykct.html

[R12] for 遍历文件
来源：http://hz.sufxvd.cn/gtmthoqiai.html

for f in *.txt; do echo "$f"; done
来源：http://hz.kuanghao11.cn/gtvlwnbkum.html

[R13] for 计数循环
来源：http://hz.birdmap.top/gtrfiwfhre.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.zdqjudy.top/gtgevuqbaz.html

[R14] C 风格 for
来源：http://hz.yvedp.cn/gtiplurwli.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.nanxinkj.top/gtgfftkpkb.html

[R15] while 逐行读文件
来源：http://hz.feifeiyinyue.top/gtyljklduq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.aibaodan.cn/gtqokdvnba.html

[R16] until 等待条件
来源：http://hz.ybcxt.top/gtynfuijcy.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.jinghuilouyu.cn/gtuzbsamgw.html

[R17] 数组定义与取值
来源：http://hz.jinqigufen.top/gtdokoopdv.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.cqqwz.cn/gtragwnxwu.html

[R18] 遍历数组
来源：http://hz.nanxinkj.top/gtksdywdsb.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.daria6918.cn/gtenwqsdxp.html

[R19] 数组长度
来源：http://hz.hnqzz.top/gtoigcglnn.html

echo "${#arr[@]}"
来源：http://hz.hnxiangtu.top/gttkoekgti.html

[R20] 关联数组（字典）
来源：http://hz.haohaochexian.top/gtqfzaulxf.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.hammf.cn/gtpffdhrij.html

[R21] 字符串长度
来源：http://hz.chenlongwang.top/gtjfjkvoxn.html

echo "${#s}"
来源：http://hz.havefunace.top/gtmvjfzlyc.html

[R22] 截取子串
来源：http://hz.zhixingplan.top/gtatyjsdug.html

echo "${s:0:5}"
来源：http://hz.yj202588.top/gtgwaxjdgo.html

[R23] 字符串替换
来源：http://hz.shanyushiyangkeji.top/gtgiqxmqxd.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.andypj.xyz/gtqpzqdpbp.html

[R24] 大小写转换
来源：http://hz.birdmap.top/gtazfozmxi.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.yangfankeji.com/gttqamevwj.html

[R25] 去后缀 / 去前缀
来源：http://hz.yueranfly.top/gtaycertfo.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.dashuyun.cn/gtdaorbyjt.html

[R26] 命令替换
来源：http://hz.haohaochexian.top/gtvpvngsxn.html

now=$(date +%F); echo "$now"
来源：http://hz.jinqigufen.top/gtjuxpmacd.html

[R27] 算术展开
来源：http://hz.xinyue.icu/gtdizcgyxh.html

echo $((1 + 2 * 3))
来源：http://hz.snrcjt.cn/gtuoegedpl.html

[R28] 浮点运算
来源：http://hz.zhaomingkeji.xyz/gtgozlgmed.html

echo "scale=2; 10/3" | bc
来源：http://hz.shuidangran.top/gtqlsovprf.html

[R29] 定义函数
来源：http://hz.ppjwa.cn/gtoxlrnaze.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.fengsongda.top/gtfkvinekd.html

[R30] 函数返回状态码
来源：http://hz.jianghu66.top/gtitmiodrt.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.xuetiantiany.cn/gtzygvcpme.html

[R31] 局部变量
来源：http://hz.andypj.xyz/gtqsxcluhd.html

f() { local x=1; echo "$x"; }
来源：http://hz.zhaomingkeji.xyz/gtlvykakst.html

[R32] 参数个数校验
来源：http://hz.dashuyun.cn/gtjlklhofk.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.svipenyu.cn/gtcxobouhj.html

[R33] 捕获错误并提示行号
来源：http://hz.cashguo.top/gtcpvvpadb.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.shzxlz.cn/gtsmmhuqtb.html

[R34] 退出时清理
来源：http://hz.bjfxy.top/gttulbblax.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.zhiwuduotai.top/gtqhjbwhvw.html

[R35] 后台执行并等待
来源：http://hz.xinyue.icu/gtjokeaqol.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.chenjidiqi.icu/gtseeypwmo.html

[R36] 并发执行多个任务
来源：http://hz.pengpengdd.cyou/gtqyguygqi.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.chenlongwang.top/gtmyxcznfj.html

[R37] 把输出赋给变量
来源：http://hz.sxryk.cn/gtkkxmtnpl.html

files=$(ls -1)
来源：http://hz.guannengcc.top/gtldpwqjkc.html

[R38] 管道串联
来源：http://hz.chenjidiqi.icu/gtzfypobah.html

cat a.txt | grep -i error | wc -l
来源：http://hz.zhongyouzk.top/gttbweodkl.html

[R39] 重定向标准输出与错误
来源：http://hz.ybcxt.top/gttadzxqfo.html

cmd > out.log 2>&1
来源：http://hz.nanxuanxn.top/gtietkxfmy.html

[R40] 追加写日志
来源：http://hz.yueranfly.top/gtjjkyoljr.html

echo "log" >> out.log
来源：http://hz.xuetiantiany.cn/gtgzdygick.html

[R41] 丢弃输出
来源：http://hz.hywenlv.cn/gtdgvtljhb.html

cmd >/dev/null 2>&1
来源：http://hz.cashguo.top/gtjsppxdxr.html

[R42] 输入重定向
来源：http://hz.tianlin.xyz/gtazfivnus.html

wc -l < a.txt
来源：http://hz.guannengcc.top/gtekaaxiwl.html

[R43] 按名字查找文件
来源：http://hz.9152youxi.cn/gtngvcucqi.html

find . -name "*.log" -type f
来源：http://hz.birdmap.top/gtjbdhkran.html

[R44] 按修改时间查找
来源：http://hz.0kj1m.cn/gtrdwyngdc.html

find . -mtime -7 -type f
来源：http://hz.cucudq.cn/gtvikmqoqw.html

[R45] 批量删除
来源：http://hz.hnqzz.top/gtcmpcyzbj.html

find . -name "*.tmp" -delete
来源：http://hz.cqqwz.cn/gtokfejnol.html

[R46] 递归替换文件内容
来源：http://hz.gzhubu.top/gtxyxctjfc.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.chenzaomai.com/gtoxzvnvpl.html

[R47] sed 单行替换
来源：http://hz.zhixingplan.top/gtbcdrmhpx.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.ivvv.top/gthprjivhw.html

[R48] awk 取指定列
来源：http://hz.hongshengwenyu.top/gtjkkbhjzc.html

awk '{print $1, $3}' a.txt
来源：http://hz.pengpengdd.cyou/gtgzqfokqs.html

[R49] awk 带条件
来源：http://hz.haohaochexian.top/gtgaqchkxl.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.guannengcc.top/gtcqsqxnuh.html

[R50] awk 求和
来源：http://hz.havefunace.top/gtuwcpkfxa.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.yonumen.top/gtpxzleyxj.html

[R51] 排序去重取前几
来源：http://hz.yangfankeji.com/gthbdbxgbq.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.chenzaomai.com/gtchxiuxwm.html

[R52] 统计行数
来源：http://hz.nanxuanxn.top/gtfdekmygy.html

wc -l a.txt
来源：http://hz.zhiwuduotai.top/gtnnevttwi.html

[R53] 查看文件头与实时尾
来源：http://hz.jinqigufen.top/gtmsnmnjtl.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.zhijiandao.cn/gtuwylhvgb.html

[R54] 比较两个文件
来源：http://hz.hnxiangtu.top/gtsltlwxqt.html

diff a.txt b.txt
来源：http://hz.yongpay.top/gtkqfmufuv.html

[R55] 压缩与解压
来源：http://hz.cdnleiting.top/gtlkrubiqd.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.dashuyun.cn/gtdpkodkog.html

[R56] 远程拷贝
来源：http://hz.9152youxi.cn/gtfvlqnnjo.html

scp file user@host:/path/
来源：http://hz.c1oappe.top/gtbmpqksmq.html

[R57] 远程执行命令
来源：http://hz.52xcode.cn/gtjzhecoww.html

ssh user@host 'uptime'
来源：http://hz.feifeiyinyue.top/gtllrsgjid.html

[R58] 下载文件
来源：http://hz.jianghu66.top/gtfutgfqxy.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.jinqigufen.top/gtovyeuzac.html

[R59] 发 POST JSON
来源：http://hz.yonumen.top/gtlipujsml.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.wangshuangyany.cn/gtjkiuafmf.html

[R60] 只看 HTTP 状态码
来源：http://hz.cqqwz.cn/gtmdgdlkco.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.gotoacloud.top/gtfyjgbquf.html

[R61] 磁盘占用
来源：http://hz.gogol.net.cn/gtszepwskl.html

df -h;  du -sh *
来源：http://hz.chenlongwang.top/gtrzqkzsmx.html

[R62] 找最占空间的文件
来源：http://hz.yj20258888.top/gtubxmzmmm.html

du -ah . | sort -rh | head -10
来源：http://hz.wangshuangyany.cn/gtamqhztjp.html

[R63] 内存与进程
来源：http://hz.yonumen.top/gtketrlprd.html

free -h;  ps aux | grep nginx
来源：http://hz.zhixingplan.top/gtmcrwtnar.html

[R64] 结束进程
来源：http://hz.316326.xyz/gtoagrlrnf.html

kill -9 $(pgrep -f app.py)
来源：http://hz.chenlongwang.top/gtmhxtkxvz.html

[R65] 查看端口占用
来源：http://hz.kuanghao11.cn/gtqjgkcprp.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.ivvv.top/gtdnqdygnd.html

[R66] 定时任务
来源：http://hz.jqgfzy.top/gtaqcoiyoy.html

crontab -e;  crontab -l
来源：http://hz.yj20258888.top/gtpnpdmxgo.html

[R67] 生成随机十六进制串
来源：http://hz.316326.xyz/gtjnkicmed.html

openssl rand -hex 16
来源：http://hz.gotoacloud.top/gtmhsutrqc.html

[R68] 计算文件校验值
来源：http://hz.mhx1999.top/gtantkzune.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.haohaochexian.top/gtlfmwwevt.html

[R69] 生成随机密码
来源：http://hz.daxiang520.top/gtkoawkqez.html

head -c 16 /dev/urandom | base64
来源：http://hz.zhengqikj.top/gtmapgppau.html

[R70] 时间戳与互转
来源：http://hz.daria6918.cn/gtfzvbidiz.html

date +%s;  date -d @1700000000
来源：http://hz.daxiang520.top/gtuhzefnoa.html

[R71] 日期格式化
来源：http://hz.yvedp.cn/gthqshkpij.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.gzhubu.top/gtunregbis.html

[R72] 等待端口就绪
来源：http://hz.jinghuilouyu.cn/gtecvmjkkz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.zhoulong.xyz/gthnsifjbg.html

[R73] 分割大日志
来源：http://hz.gotoacloud.top/gtvqjvyzim.html

split -l 1000 big.log part_
来源：http://hz.nanxinkj.top/gtsdznccfc.html

[R74] 批量重命名
来源：http://hz.wangdashe.top/gteqnxhirh.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.mhx1999.top/gtherylfpj.html

[R75] 导出环境变量
来源：http://hz.0kj1m.cn/gtkxlbhnki.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.nanxinkj.top/gtqtsxrneu.html

[R76] 使用临时文件
来源：http://hz.zhiwuduotai.top/gtnalzcjii.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.xuanzx.com/gtkqplukxs.html

[R77] 读取用户输入
来源：http://hz.pycfn.com/gtbghkbsrz.html

read -rp "请输入: " ans
来源：http://hz.cashguo.top/gtiyofcveg.html

[R78] 交互式菜单
来源：http://hz.jinqigufen.top/gtdgzlhocq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.fengsongda.top/gtgqxpgokh.html

[R79] 解析命令行选项
来源：http://hz.tian-w.cn/gtgzlvyqsl.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.chenlongwang.top/gtdeowcrpg.html

[R80] 查看脚本执行耗时
来源：http://hz.jyoumei.cn/gtnezgkfjs.html

time ./run.sh
来源：http://hz.xinyue.icu/gtagpaovpd.html

================================================================================
来源：http://hz.zhixingplan.top/gtdobddakt.html

S. C / C++ 专题
来源：http://hz.jinyuanbaomall.cn/gtunirnbka.html

================================================================================
来源：http://hz.zhongyouzk.top/gtqqkxbjmz.html

[S01] C：Hello World
来源：http://hz.nanxinkj.top/gtwacyywvq.html

#include <stdio.h>
来源：http://hz.hnxiangtu.top/gthqqpfzng.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.yvedp.cn/gtklflunqd.html

[S02] C：变量与格式化输出
来源：http://hz.aibaodan.cn/gtswistvil.html

int a = 10; printf("%d\n", a);
来源：http://hz.zdqjudy.top/gtefczbbgz.html

[S03] C：读入整数
来源：http://hz.hfpthk.cn/gtrxpmptvg.html

int x; scanf("%d", &x);
来源：http://hz.cucudq.cn/gtolbcezwz.html

[S04] C：字符串复制
来源：http://hz.zhongyouzk.top/gtgquqxbzr.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.gogol.net.cn/gtgvughhua.html

[S05] C：字符串长度
来源：http://hz.fengsongda.top/gtgrcocqqk.html

strlen(s)
来源：http://hz.jinqigfzy.top/gtuxhvzjds.html

[S06] C：字符串比较
来源：http://hz.jiagoushi.top/gttqzexapz.html

strcmp(a, b) == 0
来源：http://hz.jyoumei.cn/gtevryqsaj.html

[S07] C：数组遍历求和
来源：http://hz.hnqzz.top/gtqhycrapp.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.jinqigufen.top/gtfexpyluf.html

[S08] C：动态内存分配与释放
来源：http://hz.xuanzx.com/gtgsmdqppi.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.gotoacloud.top/gthocwyble.html

[S09] C：结构体定义与初始化
来源：http://hz.pycfn.com/gtjzoujhpt.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.birdmap.top/gthzfuqlol.html

[S10] C：指针与解引用
来源：http://hz.pycfn.com/gtvnvknlfp.html

int *p = &a;  *p = 5;
来源：http://hz.yj20258888.top/gtoetrqwgg.html

[S11] C：逐行读文件
来源：http://hz.dianchejie.cn/gtkwhddjiv.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.wangshuangyany.cn/gtjboigycm.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.vqdsnc.cn/gtswwvswoo.html

fclose(f);
来源：http://hz.birdmap.top/gtrfvlnqqc.html

[S12] C：写文件
来源：http://hz.guannengcc.top/gtazjpspvw.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.quarkkingdee.top/gtpxklpipz.html

[S13] C：宏定义
来源：http://hz.jlsjyb.cn/gtrzznhfzx.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.snrcjt.cn/gtvjojldln.html

[S14] C：枚举
来源：http://hz.hnqzz.top/gtzpngjgmm.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.sweek.top/gtjbbbnqoq.html

[S15] C：类型转换
来源：http://hz.fengsongda.top/gtcnsmyjic.html

(double) a / b
来源：http://hz.jinqigufen.top/gtdemeshzr.html

[S16] C：位操作置位
来源：http://hz.316326.xyz/gtxvjeqxpe.html

x |= (1 << 3);
来源：http://hz.hammf.cn/gtgtbrxwxe.html

[S17] C：安全拼接字符串
来源：http://hz.pycfn.com/gtrbvohlhz.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.chenjidiqi.icu/gtplvbhgmm.html

[S18] C：命令行参数
来源：http://hz.jinyuanbaomall.cn/gtsffjoyta.html

int main(int argc, char **argv)
来源：http://hz.tanke756.top/gtrkdjpxub.html

[S19] C：快速排序
来源：http://hz.yongpay.top/gtflgsemee.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.xinyue.icu/gtwnzlysxw.html

[S20] C：二分查找
来源：http://hz.guowangkeji.top/gtugkzbdkh.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.nanxuanxn.top/gtnjdselnr.html

[S21] C：字符类别判断
来源：http://hz.zhengqikj.top/gtzaepimlh.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.haohaochexian.top/gtmdllpcnh.html

[S22] C：字符串转数字
来源：http://hz.yj20258.top/gtdwsulryx.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.gogol.net.cn/gtzlfodwhh.html

[S23] C：随机数
来源：http://hz.jqgfzy.top/gtkhcgfvul.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.sufxvd.cn/gtvgoxzwkq.html

[S24] C：获取本地时间
来源：http://hz.hammf.cn/gttrmjzbch.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.mhx1999.top/gtklvhruyn.html

[S25] C：内存拷贝
来源：http://hz.xingfuxueyuan.xyz/gtbcgupfsd.html

memcpy(dst, src, n);
来源：http://hz.sweek.top/gtnhmebjbt.html

[S26] C：内存清零
来源：http://hz.meibo888.top/gtbyxvzvbp.html

memset(a, 0, sizeof a);
来源：http://hz.yangfankeji.com/gtetwqqwbb.html

[S27] C：定义常量
来源：http://hz.gzhubu.top/gtmkutofhx.html

const double PI = 3.14159;
来源：http://hz.yj20258.top/gtymegjkhg.html

[S28] C：静态变量
来源：http://hz.hongshengwenyu.top/gtilwvwghm.html

static int counter = 0;
来源：http://hz.wangshuangyany.cn/gtlzqtnekh.html

[S29] C：变参函数
来源：http://hz.meibo888.top/gtihgldjzm.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.jinyuanbaomall.cn/gtfpdwxhpn.html

[S30] C：头文件保护
来源：http://hz.chenlongwang.top/gtatlljkql.html

#ifndef X_H
来源：http://hz.iojbl.cn/gtcxwjwxmi.html

#define X_H
来源：http://hz.ehwqpu.com/gthyqssezg.html

#endif
来源：http://hz.9152youxi.cn/gtnwforjwh.html

[S31] C++：Hello World
来源：http://hz.fzhhl.top/gtwkxhwtpk.html

#include <iostream>
来源：http://hz.xylfe.cn/gtwaopvuyp.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.yj20258888.top/gtshnxnvjc.html

[S32] C++：字符串
来源：http://hz.daria6918.cn/gtyggtczsa.html

std::string s = "hi";  s += "!";
来源：http://hz.gogol.net.cn/gtawboutud.html

[S33] C++：vector 增删
来源：http://hz.shangyingyoupin.top/gtmtfjxrix.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.tian-w.cn/gtzdyhiqft.html

[S34] C++：遍历 vector
来源：http://hz.cdnleiting.top/gtxoipsbou.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.0kj1m.cn/gtwllbxfja.html

[S35] C++：map
来源：http://hz.zhijiandao.cn/gtcjondezq.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.tian-w.cn/gtkjzcjisg.html

[S36] C++：unordered_map
来源：http://hz.shzxlz.cn/gtxehrzliw.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.xuanzx.com/gteuqibcyh.html

[S37] C++：set
来源：http://hz.zhongyouzk.top/gtyebvbwgk.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.aizwys.cn/gtjtmoppmv.html

[S38] C++：排序
来源：http://hz.meibo888.top/gtykvddkyh.html

std::sort(v.begin(), v.end());
来源：http://hz.cucudq.cn/gtxwsehksb.html

[S39] C++：自定义比较器排序
来源：http://hz.jinghuilouyu.cn/gtpsswoyma.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.316326.xyz/gtyrtiwuqd.html

[S40] C++：查找元素
来源：http://hz.hnqzz.top/gtttemcrla.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.dashuyun.cn/gtwdmwqoon.html

[S41] C++：类与构造函数
来源：http://hz.hywenlv.cn/gtwhsbzypp.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.cdnleiting.top/gttszirzae.html

[S42] C++：继承与虚函数
来源：http://hz.xuetiantiany.cn/gtpdhkobja.html

class B : public Base { public: void f() override {} };
来源：http://hz.fengsongda.top/gtruhktssn.html

[S43] C++：智能指针
来源：http://hz.chenlongwang.top/gtjnvdxoyr.html

auto p = std::make_unique<int>(5);
来源：http://hz.aizwys.cn/gtnkiaybkg.html

[S44] C++：引用传参
来源：http://hz.hnqzz.top/gtbasqykbo.html

void inc(int &x) { ++x; }
来源：http://hz.shzxlz.cn/gtfqulqqvw.html

[S45] C++：lambda
来源：http://hz.ybcxt.top/gtnrzfjxmg.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.shanyushiyangkeji.top/gthlvbzmho.html

[S46] C++：函数模板
来源：http://hz.c1oappe.top/gtetjredpn.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.redwolf501.top/gttaclxugg.html


<!-- 参考信息 -->