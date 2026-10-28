代发 wailian999

ANALYZE TABLE users;
来源：http://hz.shzxlz.cn/gtkgxfgfyt.html

[Q71] 查看建表语句
来源：http://hz.jinqigfzy.top/gtrifhgluk.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.chenjidiqi.icu/gtyvzmjrog.html

[Q72] 查看索引
来源：http://hz.yj20258.top/gtwnujfvpm.html

SHOW INDEX FROM users;
来源：http://hz.cdnleiting.top/gtgqyljhch.html

[Q73] 查看表状态
来源：http://hz.dianchejie.cn/gtlqmytfnf.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.yj20258.top/gtzaeckhyv.html

[Q74] 强制使用索引
来源：http://hz.cucudq.cn/gtmuorvxvv.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.hywenlv.cn/gtduedgtla.html

[Q75] 日期格式化
来源：http://hz.cucudq.cn/gtbupfjgqm.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.xylfe.cn/gttmdbjmke.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.redwolf501.top/gthfmcbnow.html

[Q76] 按天统计
来源：http://hz.cheryme.top/gtbyfxaebi.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.gotoacloud.top/gtvmnrzgdo.html

[Q77] 时间加减
来源：http://hz.hongshengwenyu.top/gtotwefimn.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.andypj.xyz/gtwtybwclf.html

[Q78] 当前时间
来源：http://hz.ybcxt.top/gthyaqtfcf.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.ehwqpu.com/gtitsykgrm.html

[Q79] 字符串拼接
来源：http://hz.yongpay.top/gttltwlmgz.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.iojbl.cn/gtmvreetro.html

[Q80] 字符串截取
来源：http://hz.gaohongyu789.top/gtuuukdpho.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.meibo888.top/gtkcsyogzu.html

[Q81] 字符串替换
来源：http://hz.yueranfly.top/gtbcvyqggb.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.zhoulong.xyz/gtrtxxfmik.html

[Q82] 字符长度与字节长度
来源：http://hz.xziqi.cn/gtxqddjamx.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.jinqigufen.top/gtlnynxkqm.html

[Q83] 大小写转换
来源：http://hz.yanxiufei.cn/gtucftgfux.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.ywan-chungtsiang.top/gticgohkik.html

[Q84] 去除首尾空格
来源：http://hz.yvedp.cn/gtvmotlnyk.html

SELECT TRIM(name) FROM users;
来源：http://hz.52xcode.cn/gthextvube.html

[Q85] 数值取整
来源：http://hz.haohaochexian.top/gtdohrptll.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.yvedp.cn/gttsbjrrlx.html

[Q86] 读取 JSON 字段
来源：http://hz.shzxlz.cn/gttszrenci.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.316326.xyz/gtswrzsfcy.html

[Q87] JSON 字段做条件
来源：http://hz.xuanzx.com/gtznfapvjp.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.jinyuanbaomall.cn/gtsycjiazv.html

[Q88] 行转列（条件聚合）
来源：http://hz.shanyushiyangkeji.top/gtvssddydb.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.jinyuanbaomall.cn/gtpqfytlak.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.nwbrower.top/gtxoglcsby.html

[Q89] 判断表是否存在
来源：http://hz.redwolf501.top/gtcpsftuym.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.jinqigfzy.top/gtvtccbfcp.html

[Q90] 生成序号列
来源：http://hz.0kj1m.cn/gtburemqnm.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.andypj.xyz/gtgtrzvtce.html

================================================================================
来源：http://hz.vqdsnc.cn/gtwfitiyge.html

R. Bash 专题
来源：http://hz.jinqigfzy.top/gtnyrufbxu.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtrmmlpkcd.html

[R01] shebang 与严格模式
来源：http://hz.guannengcc.top/gtjnrablmo.html

#!/usr/bin/env bash
来源：http://hz.dianchejie.cn/gtaxjcrflb.html

set -euo pipefail
来源：http://hz.xylfe.cn/gtgktvkibn.html

[R02] 变量赋值与使用
来源：http://hz.xuetiantiany.cn/gtmuihrfjk.html

name="Tom"; echo "$name"
来源：http://hz.pengpengdd.cyou/gtjwlvdgeo.html

[R03] 只读变量
来源：http://hz.zhiwuduotai.top/gtbnhulhra.html

readonly PI=3.14
来源：http://hz.aibaodan.cn/gtrnxzizpc.html

[R04] 位置参数
来源：http://hz.snrcjt.cn/gtdwzeuobw.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.xuanzx.com/gtviifclsu.html

[R05] 参数默认值
来源：http://hz.cdnleiting.top/gtiilswokh.html

name="${1:-default}"
来源：http://hz.ydjk.org.cn/gtmeopaidd.html

[R06] 判断命令是否存在
来源：http://hz.kuanghao11.cn/gticnvqcbo.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.zhengqikj.top/gtwnkyxqgw.html

[R07] if 判断文件
来源：http://hz.bjfxy.top/gtiuwefwpz.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.yanxiufei.cn/gtpmmoueip.html

[R08] 数值比较
来源：http://hz.chenjidiqi.icu/gthugdcluu.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.xylfe.cn/gtcegfdmxc.html

[R09] 字符串比较
来源：http://hz.iojbl.cn/gtnfqgjftc.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.yuanzhike.top/gtwowjurrq.html

[R10] 正则匹配
来源：http://hz.hfpthk.cn/gtbggumptc.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.cqqwz.cn/gtzardtsgo.html

[R11] case 多分支
来源：http://hz.feifeiyinyue.top/gtmetfdbvk.html

case "$1" in
来源：http://hz.dashuyun.cn/gtazjbzgtj.html

start) echo "启动" ;;
来源：http://hz.andypj.xyz/gtibdcgmed.html

stop)  echo "停止" ;;
来源：http://hz.jinyuanbaomall.cn/gtkzhnjize.html

*)     echo "未知命令" ;;
来源：http://hz.hfpthk.cn/gtihhumity.html

esac
来源：http://hz.yuxming.cn/gteonowmst.html

[R12] for 遍历文件
来源：http://hz.jinqigufen.top/gtxdxbtnoz.html

for f in *.txt; do echo "$f"; done
来源：http://hz.shanyushiyangkeji.top/gtywnnxbuv.html

[R13] for 计数循环
来源：http://hz.hnqzz.top/gtlzisnnjj.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.vqdsnc.cn/gtqasjgrim.html

[R14] C 风格 for
来源：http://hz.jinghuilouyu.cn/gtooexjagb.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.feifeiyinyue.top/gtschzyafs.html

[R15] while 逐行读文件
来源：http://hz.svipenyu.cn/gtzuywrkfm.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.xingfuxueyuan.xyz/gtkbdncoaj.html

[R16] until 等待条件
来源：http://hz.kuanghao11.cn/gtpzbjhjrs.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.chenjidiqi.icu/gtonjgihiw.html

[R17] 数组定义与取值
来源：http://hz.yuxming.cn/gtzpvkjsko.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.cdnleiting.top/gtmasvjyph.html

[R18] 遍历数组
来源：http://hz.meibo888.top/gtfcpwgnbv.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.ybcxt.top/gtknxazspp.html

[R19] 数组长度
来源：http://hz.cheryme.top/gtzmskkhoq.html

echo "${#arr[@]}"
来源：http://hz.smart0.xyz/gtfqtgtknd.html

[R20] 关联数组（字典）
来源：http://hz.fengsongda.top/gtyxcbadfm.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.meibo888.top/gtmzyclngf.html

[R21] 字符串长度
来源：http://hz.xuanzx.com/gtmggagxww.html

echo "${#s}"
来源：http://hz.tianlin.xyz/gtahjwjkci.html

[R22] 截取子串
来源：http://hz.9152youxi.cn/gtcpzoynft.html

echo "${s:0:5}"
来源：http://hz.9152youxi.cn/gthdgfnqnr.html

[R23] 字符串替换
来源：http://hz.andypj.xyz/gtneqjrhxu.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.jyoumei.cn/gtwikucbmd.html

[R24] 大小写转换
来源：http://hz.shanyushiyangkeji.top/gtwidhevtu.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.nanxinkj.top/gtltemqdbb.html

[R25] 去后缀 / 去前缀
来源：http://hz.yj20258888.top/gtleipfuxg.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.0kj1m.cn/gtguoebisg.html

[R26] 命令替换
来源：http://hz.yonumen.top/gtalenfwkf.html

now=$(date +%F); echo "$now"
来源：http://hz.sxryk.cn/gtppttiksa.html

[R27] 算术展开
来源：http://hz.shzxlz.cn/gthzdpspah.html

echo $((1 + 2 * 3))
来源：http://hz.cashguo.top/gtqzyihtds.html

[R28] 浮点运算
来源：http://hz.9152youxi.cn/gtokwsgyie.html

echo "scale=2; 10/3" | bc
来源：http://hz.chenjidiqi.icu/gtuyfkkaqp.html

[R29] 定义函数
来源：http://hz.wangdashe.top/gtehocxdsj.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.jyoumei.cn/gtyemwdtfl.html

[R30] 函数返回状态码
来源：http://hz.ehwqpu.com/gtiyjfiowj.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.redwolf501.top/gtbttkngnt.html

[R31] 局部变量
来源：http://hz.xinyue.icu/gtowfjawyi.html

f() { local x=1; echo "$x"; }
来源：http://hz.guannengcc.top/gtjbjwrwuj.html

[R32] 参数个数校验
来源：http://hz.hnxiangtu.top/gtgfosxpmf.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.dianchejie.cn/gtonjitwbs.html

[R33] 捕获错误并提示行号
来源：http://hz.hammf.cn/gtjkhmruiw.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.yj20258.top/gtbpyeasjm.html

[R34] 退出时清理
来源：http://hz.ydjk.org.cn/gtvgbgxhfp.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.yanxiufei.cn/gtgttabdxk.html

[R35] 后台执行并等待
来源：http://hz.kuanghao11.cn/gtyiwisvhz.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.hywenlv.cn/gtvrfjxlta.html

[R36] 并发执行多个任务
来源：http://hz.hnqzz.top/gtlvflqorl.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.shanyushiyangkeji.top/gtnqmfqyuw.html

[R37] 把输出赋给变量
来源：http://hz.shanyushiyangkeji.top/gtbmcsoqcd.html

files=$(ls -1)
来源：http://hz.zycfv.cn/gteolcgytt.html

[R38] 管道串联
来源：http://hz.shzxlz.cn/gtpxkxsumn.html

cat a.txt | grep -i error | wc -l
来源：http://hz.zhengqikj.top/gtuibnalrr.html

[R39] 重定向标准输出与错误
来源：http://hz.chenzaomai.com/gtthdsbybe.html

cmd > out.log 2>&1
来源：http://hz.hnxiangtu.top/gtaqerjpap.html

[R40] 追加写日志
来源：http://hz.ywan-chungtsiang.top/gtkjioipyp.html

echo "log" >> out.log
来源：http://hz.quarkkingdee.top/gtdyokpetv.html

[R41] 丢弃输出
来源：http://hz.jqgfzy.top/gtvtqcabem.html

cmd >/dev/null 2>&1
来源：http://hz.chenlongwang.top/gttzyjihnk.html

[R42] 输入重定向
来源：http://hz.xuetiantiany.cn/gtgmycwptw.html

wc -l < a.txt
来源：http://hz.jinqigufen.top/gtxaaimnvu.html

[R43] 按名字查找文件
来源：http://hz.cheryme.top/gtqimxupgf.html

find . -name "*.log" -type f
来源：http://hz.vqdsnc.cn/gtbhicoczc.html

[R44] 按修改时间查找
来源：http://hz.cdnleiting.top/gtxkpkznow.html

find . -mtime -7 -type f
来源：http://hz.yuxming.cn/gtwoqjsghp.html

[R45] 批量删除
来源：http://hz.aibaodan.cn/gtawgphuuo.html

find . -name "*.tmp" -delete
来源：http://hz.shanyushiyangtech.top/gtbmeammqo.html

[R46] 递归替换文件内容
来源：http://hz.ehwqpu.com/gtyxgfjdjp.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.xuanzx.com/gtfkwungxb.html

[R47] sed 单行替换
来源：http://hz.havefunace.top/gtbkireyba.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.sufxvd.cn/gtlyogbpwp.html

[R48] awk 取指定列
来源：http://hz.ywan-chungtsiang.top/gtorvllakl.html

awk '{print $1, $3}' a.txt
来源：http://hz.cashguo.top/gtfckmrods.html

[R49] awk 带条件
来源：http://hz.ivvv.top/gtjafixthi.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.zdqjudy.top/gtalltsuxf.html

[R50] awk 求和
来源：http://hz.xuanzx.com/gticwgnjkn.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.shuidangran.top/gtisqdmaor.html

[R51] 排序去重取前几
来源：http://hz.jinghuilouyu.cn/gtwtfdqquv.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.jyoumei.cn/gttfrnpcjk.html

[R52] 统计行数
来源：http://hz.gogol.net.cn/gtcdkcgylv.html

wc -l a.txt
来源：http://hz.chenjidiqi.icu/gtoighcjxa.html

[R53] 查看文件头与实时尾
来源：http://hz.xziqi.cn/gtiewgsqxb.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.chenzaomai.com/gthvovxqvz.html

[R54] 比较两个文件
来源：http://hz.chenzaomai.com/gtltmpowzd.html

diff a.txt b.txt
来源：http://hz.jqgfzy.top/gtmvkuylli.html

[R55] 压缩与解压
来源：http://hz.yongpay.top/gtqtxcgyka.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.zycfv.cn/gtkfqbesuq.html

[R56] 远程拷贝
来源：http://hz.cqqwz.cn/gtrzxoachx.html

scp file user@host:/path/
来源：http://hz.ppjwa.cn/gtnpeofqro.html

[R57] 远程执行命令
来源：http://hz.sysykeji.top/gtegsehzbl.html

ssh user@host 'uptime'
来源：http://hz.52xcode.cn/gtrvvibwft.html

[R58] 下载文件
来源：http://hz.yongpay.top/gtaempwxds.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.pycfn.com/gtpeqhcbkp.html

[R59] 发 POST JSON
来源：http://hz.andypj.xyz/gtgztexlql.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.zhaomingkeji.xyz/gtvizecvjh.html

[R60] 只看 HTTP 状态码
来源：http://hz.hfpthk.cn/gthhqciuic.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.hfpthk.cn/gtmpekdajq.html

[R61] 磁盘占用
来源：http://hz.xingfuxueyuan.xyz/gtzdkeysay.html

df -h;  du -sh *
来源：http://hz.chenjidiqi.icu/gtkrzdvtyq.html

[R62] 找最占空间的文件
来源：http://hz.pycfn.com/gtfstplpce.html

du -ah . | sort -rh | head -10
来源：http://hz.shanyushiyangkeji.top/gtnhmnmeki.html

[R63] 内存与进程
来源：http://hz.jinqigufen.top/gtusjfyrel.html

free -h;  ps aux | grep nginx
来源：http://hz.iojbl.cn/gtkeczosej.html

[R64] 结束进程
来源：http://hz.shuidangran.top/gtvjzfpeqc.html

kill -9 $(pgrep -f app.py)
来源：http://hz.zhiwuduotai.top/gtgxnkllat.html

[R65] 查看端口占用
来源：http://hz.ppjwa.cn/gtsmnzgwlz.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.chenzaomai.com/gtljgjotml.html

[R66] 定时任务
来源：http://hz.jqgfzy.top/gtnkknehto.html

crontab -e;  crontab -l
来源：http://hz.hfpthk.cn/gtmdviovpg.html

[R67] 生成随机十六进制串
来源：http://hz.kuanghao11.cn/gtdhbtynab.html

openssl rand -hex 16
来源：http://hz.jyoumei.cn/gtvaxnlpjs.html

[R68] 计算文件校验值
来源：http://hz.zhongyouzk.top/gtdsmezyli.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.zhoulong.xyz/gtlggihype.html

[R69] 生成随机密码
来源：http://hz.xylfe.cn/gtutohbagt.html

head -c 16 /dev/urandom | base64
来源：http://hz.hammf.cn/gtmgsailnd.html

[R70] 时间戳与互转
来源：http://hz.gogol.net.cn/gtvlkfaskq.html

date +%s;  date -d @1700000000
来源：http://hz.xinyue.icu/gthqmzykjg.html

[R71] 日期格式化
来源：http://hz.hammf.cn/gtcbbwptzd.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.jlsjyb.cn/gtrxwqvbvo.html

[R72] 等待端口就绪
来源：http://hz.xziqi.cn/gtzhgzjupr.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.zhijiandao.cn/gtrgbdqqiy.html

[R73] 分割大日志
来源：http://hz.dianchejie.cn/gtmwuqamxp.html

split -l 1000 big.log part_
来源：http://hz.nwbrower.top/gtarhrfouv.html

[R74] 批量重命名
来源：http://hz.zhixingplan.top/gtqfaatfmx.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.wangshuangyany.cn/gtvaxcaarr.html

[R75] 导出环境变量
来源：http://hz.cheryme.top/gtgpfexzuc.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.birdmap.top/gtybazxshd.html

[R76] 使用临时文件
来源：http://hz.zycfv.cn/gttiahzjvw.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.meibo888.top/gtsrhzmkaq.html

[R77] 读取用户输入
来源：http://hz.tianlin.xyz/gtxrjcpjkq.html

read -rp "请输入: " ans
来源：http://hz.xuanzx.com/gtlqvulbia.html

[R78] 交互式菜单
来源：http://hz.xylfe.cn/gtxzekneeo.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.chenjidiqi.icu/gteujevdzm.html

[R79] 解析命令行选项
来源：http://hz.bjfxy.top/gtwponmerw.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.jianghu66.top/gtvwvinvwn.html

[R80] 查看脚本执行耗时
来源：http://hz.ywan-chungtsiang.top/gtolppdnbf.html

time ./run.sh
来源：http://hz.sufxvd.cn/gtfmiaudjz.html

================================================================================
来源：http://hz.yj20258888.top/gtekyfzkcn.html

S. C / C++ 专题
来源：http://hz.pycfn.com/gtogkcbyud.html

================================================================================
来源：http://hz.gzhubu.top/gtnqsmohnd.html

[S01] C：Hello World
来源：http://hz.hongshengwenyu.top/gtktmwwlly.html

#include <stdio.h>
来源：http://hz.sufxvd.cn/gtaxtyiool.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.c1oappe.top/gtqgoxtwlb.html

[S02] C：变量与格式化输出
来源：http://hz.yj20258.top/gtkgevltlt.html

int a = 10; printf("%d\n", a);
来源：http://hz.hysaishi.cn/gtkjqmihgt.html

[S03] C：读入整数
来源：http://hz.xuanzx.com/gtqbddnapd.html

int x; scanf("%d", &x);
来源：http://hz.shzxlz.cn/gtphzsjfhk.html

[S04] C：字符串复制
来源：http://hz.cucudq.cn/gtdvzjkpmx.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.cucudq.cn/gtyekcsfaf.html

[S05] C：字符串长度
来源：http://hz.yongpay.top/gtybobmiah.html

strlen(s)
来源：http://hz.hysaishi.cn/gtfcvlthza.html

[S06] C：字符串比较
来源：http://hz.birdmap.top/gthwkojbho.html

strcmp(a, b) == 0
来源：http://hz.svipenyu.cn/gtwdbvwwwv.html

[S07] C：数组遍历求和
来源：http://hz.c1oappe.top/gtcpogulif.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.pycfn.com/gtldbnnjwc.html

[S08] C：动态内存分配与释放
来源：http://hz.jinghuilouyu.cn/gtkrrtysyf.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.jinyuanbaomall.cn/gtewullfuk.html

[S09] C：结构体定义与初始化
来源：http://hz.yj20258.top/gtegztjnmd.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.dashuyun.cn/gtehrwspvp.html

[S10] C：指针与解引用
来源：http://hz.daxiang520.top/gtiigssfba.html

int *p = &a;  *p = 5;
来源：http://hz.jinghuilouyu.cn/gtyzryidso.html

[S11] C：逐行读文件
来源：http://hz.zhixingplan.top/gtjqsuvigc.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.pycfn.com/gtodttpkii.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.feifeiyinyue.top/gtgxbltjxj.html

fclose(f);
来源：http://hz.nanxinkj.top/gtubsiasln.html

[S12] C：写文件
来源：http://hz.cheryme.top/gtxlffdkla.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.jinyuanbaomall.cn/gtbxffygls.html

[S13] C：宏定义
来源：http://hz.aizwys.cn/gtpsjsdwjd.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.c1oappe.top/gtmbppudrv.html

[S14] C：枚举
来源：http://hz.jinqigufen.top/gtjzzmbrdh.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.redwolf501.top/gteaqkfrhd.html

[S15] C：类型转换
来源：http://hz.xylfe.cn/gtbuqrladj.html

(double) a / b
来源：http://hz.tianlin.xyz/gtysnywege.html

[S16] C：位操作置位
来源：http://hz.sufxvd.cn/gtuamjpsvi.html

x |= (1 << 3);
来源：http://hz.52xcode.cn/gtgfikumqx.html

[S17] C：安全拼接字符串
来源：http://hz.gaohongyu789.top/gtrqpisoqn.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.wangdashe.top/gtqibsiano.html

[S18] C：命令行参数
来源：http://hz.fengsongda.top/gtaofvjrud.html

int main(int argc, char **argv)
来源：http://hz.zycfv.cn/gtyfuvyfbq.html

[S19] C：快速排序
来源：http://hz.hysaishi.cn/gtjdmjrqup.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.316326.xyz/gtlnoonqdt.html

[S20] C：二分查找
来源：http://hz.yj20258888.top/gtpioqpcal.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.52xcode.cn/gttphjjevs.html

[S21] C：字符类别判断
来源：http://hz.hysaishi.cn/gtgkujlike.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.ppjwa.cn/gtnsntbsdx.html

[S22] C：字符串转数字
来源：http://hz.yueranfly.top/gtzmxseapb.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.aibaodan.cn/gttlysrwwd.html

[S23] C：随机数
来源：http://hz.zhoulong.xyz/gtusolupdn.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.hnxiangtu.top/gtjosmtvyh.html

[S24] C：获取本地时间
来源：http://hz.birdmap.top/gtwtchlwma.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.cheryme.top/gtjjozfweh.html

[S25] C：内存拷贝
来源：http://hz.hnxiangtu.top/gtoatypjud.html

memcpy(dst, src, n);
来源：http://hz.zhengqikj.top/gtdjkcamyg.html

[S26] C：内存清零
来源：http://hz.xingfuxueyuan.xyz/gttyhzflfo.html

memset(a, 0, sizeof a);
来源：http://hz.hnqzz.top/gtlmdinvan.html

[S27] C：定义常量
来源：http://hz.yonumen.top/gtbvklctut.html

const double PI = 3.14159;
来源：http://hz.yonumen.top/gtfofrpsbj.html

[S28] C：静态变量
来源：http://hz.dashuyun.cn/gtrnqhhkmc.html

static int counter = 0;
来源：http://hz.aibaodan.cn/gtqvgphksb.html

[S29] C：变参函数
来源：http://hz.ydjk.org.cn/gthnhfehfq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.52xcode.cn/gtialsccgp.html

[S30] C：头文件保护
来源：http://hz.cqqwz.cn/gtczblordd.html

#ifndef X_H
来源：http://hz.pengpengdd.cyou/gtkfhonjip.html

#define X_H
来源：http://hz.hongshengwenyu.top/gtczixojtq.html

#endif
来源：http://hz.nwbrower.top/gtetunjboc.html

[S31] C++：Hello World
来源：http://hz.hnqzz.top/gtfunsqkmo.html

#include <iostream>
来源：http://hz.yvedp.cn/gtwwkwakpo.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.gaohongyu789.top/gtdpdekcbx.html

[S32] C++：字符串
来源：http://hz.zhijiandao.cn/gtqeifvepe.html

std::string s = "hi";  s += "!";
来源：http://hz.cashguo.top/gtpoeyteug.html

[S33] C++：vector 增删
来源：http://hz.svipenyu.cn/gtqubvbckh.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.iojbl.cn/gthicwebxs.html

[S34] C++：遍历 vector
来源：http://hz.hfpthk.cn/gtlheeocuc.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.tian-w.cn/gtnjwmmtsq.html

[S35] C++：map
来源：http://hz.gogol.net.cn/gtarjqjadu.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.svipenyu.cn/gtubiamjnj.html

[S36] C++：unordered_map
来源：http://hz.hammf.cn/gtuakcagie.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yangfankeji.com/gtqlruejbv.html

[S37] C++：set
来源：http://hz.hammf.cn/gtkhpiibwz.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.haohaochexian.top/gtjjxjtegb.html

[S38] C++：排序
来源：http://hz.pycfn.com/gtdwzwbdkl.html

std::sort(v.begin(), v.end());
来源：http://hz.cashguo.top/gtvsuskyte.html

[S39] C++：自定义比较器排序
来源：http://hz.xingfuxueyuan.xyz/gtcwadcmkj.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.yj20258.top/gtxnocttyy.html

[S40] C++：查找元素
来源：http://hz.sweek.top/gtyqjlthwe.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.jinghuilouyu.cn/gtbvyffjsp.html


<!-- 参考信息 -->