代发 wailian999

ROLLBACK TO sp1;
来源：http://hz.shuidangran.top/gtmxbijvvj.html

[Q69] 查看执行计划
来源：http://hz.daxiang520.top/gtjyxbjkiw.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.birdmap.top/gtsjmboear.html

[Q70] 更新统计信息
来源：http://hz.feifeiyinyue.top/gtfukupdcn.html

ANALYZE TABLE users;
来源：http://hz.birdmap.top/gtolwpgivy.html

[Q71] 查看建表语句
来源：http://hz.xinyue.icu/gtaupfyfrg.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.jqgfzy.top/gtwqmglefk.html

[Q72] 查看索引
来源：http://hz.cashguo.top/gtivzsnhlb.html

SHOW INDEX FROM users;
来源：http://hz.yuanzhike.top/gtlyafcnuc.html

[Q73] 查看表状态
来源：http://hz.sxryk.cn/gtlzwxgdcz.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.yanxiufei.cn/gtoatgjcfb.html

[Q74] 强制使用索引
来源：http://hz.sweek.top/gtwzdgvebf.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.tanke756.top/gturvjyzpy.html

[Q75] 日期格式化
来源：http://hz.jqgfzy.top/gtsdlvmzzh.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.cqqwz.cn/gtsitfrhjm.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.aibaodan.cn/gtgudvpfqf.html

[Q76] 按天统计
来源：http://hz.ppjwa.cn/gthcvuovab.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.zhaomingkeji.xyz/gtlmvtjdxs.html

[Q77] 时间加减
来源：http://hz.chenzaomai.com/gtrsiafbfm.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.jiagoushi.top/gtvenxodcy.html

[Q78] 当前时间
来源：http://hz.smart0.xyz/gtrbrudsox.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.cashguo.top/gtlsgzwgfu.html

[Q79] 字符串拼接
来源：http://hz.kuanghao11.cn/gttpggcodd.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.aizwys.cn/gtcuonvoxs.html

[Q80] 字符串截取
来源：http://hz.yuxming.cn/gtfexxawzx.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.zhengqikj.top/gtqqzplstb.html

[Q81] 字符串替换
来源：http://hz.316326.xyz/gtlsufdfan.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.xingfuxueyuan.xyz/gtxqlknwrg.html

[Q82] 字符长度与字节长度
来源：http://hz.iojbl.cn/gtagamdyte.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.jqgfzy.top/gtrksziqtk.html

[Q83] 大小写转换
来源：http://hz.iojbl.cn/gtufwcpgxv.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.yueranfly.top/gtmfjvpvpn.html

[Q84] 去除首尾空格
来源：http://hz.yj202588.top/gtvwyedivh.html

SELECT TRIM(name) FROM users;
来源：http://hz.daria6918.cn/gtcmfanmic.html

[Q85] 数值取整
来源：http://hz.cqqwz.cn/gtwncbamgu.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.shanyushiyangkeji.top/gthbloivvc.html

[Q86] 读取 JSON 字段
来源：http://hz.dianchejie.cn/gtyfdabryc.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.52xcode.cn/gtwszoqmpd.html

[Q87] JSON 字段做条件
来源：http://hz.cucudq.cn/gtaitbgjnm.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.yangfankeji.com/gtmrqdkggp.html

[Q88] 行转列（条件聚合）
来源：http://hz.yonumen.top/gtwwlkdcky.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.zhongyouzk.top/gtxyaughst.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.jqgufenzy.top/gtvdolnkyy.html

[Q89] 判断表是否存在
来源：http://hz.zhijiandao.cn/gtcktbadkr.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.cheryme.top/gtcdzqanla.html

[Q90] 生成序号列
来源：http://hz.dashuyun.cn/gtzvfawlcu.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.yonumen.top/gtnjvcrwqn.html

================================================================================
来源：http://hz.dashuyun.cn/gtuapjzirk.html

R. Bash 专题
来源：http://hz.xziqi.cn/gtthsvnyas.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtdgsshedz.html

[R01] shebang 与严格模式
来源：http://hz.hysaishi.cn/gtqpyioozz.html

#!/usr/bin/env bash
来源：http://hz.dashuyun.cn/gtqdjeuyux.html

set -euo pipefail
来源：http://hz.cucudq.cn/gtkepcsnyg.html

[R02] 变量赋值与使用
来源：http://hz.nanxinkj.top/gtemonmvrl.html

name="Tom"; echo "$name"
来源：http://hz.yj20258.top/gtmredasxb.html

[R03] 只读变量
来源：http://hz.gaohongyu789.top/gtoezcbkdi.html

readonly PI=3.14
来源：http://hz.jqgufenzy.top/gtyzlfsdqv.html

[R04] 位置参数
来源：http://hz.nwbrower.top/gtklyszvnr.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.snrcjt.cn/gtsgeukbvg.html

[R05] 参数默认值
来源：http://hz.daria6918.cn/gtzuqgeqbf.html

name="${1:-default}"
来源：http://hz.sweek.top/gtbvyozdhs.html

[R06] 判断命令是否存在
来源：http://hz.pycfn.com/gtuiwsfdqk.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.yj202588.top/gtavnvrwnd.html

[R07] if 判断文件
来源：http://hz.xingfuxueyuan.xyz/gtzcwuqeld.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.shanyushiyangkeji.top/gtvnbretij.html

[R08] 数值比较
来源：http://hz.52xcode.cn/gthuqpvdod.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.cdnleiting.top/gthdvxwdnt.html

[R09] 字符串比较
来源：http://hz.ydjk.org.cn/gtpqzwnzau.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.0kj1m.cn/gtqvgfzlxq.html

[R10] 正则匹配
来源：http://hz.cucudq.cn/gtoksgxctx.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.shanyushiyangtech.top/gtdmszduha.html

[R11] case 多分支
来源：http://hz.wangshuangyany.cn/gtuqooquou.html

case "$1" in
来源：http://hz.yuanzhike.top/gtkwjuddhb.html

start) echo "启动" ;;
来源：http://hz.smart0.xyz/gtpwdvjhvh.html

stop)  echo "停止" ;;
来源：http://hz.vqdsnc.cn/gtqukpjlhi.html

*)     echo "未知命令" ;;
来源：http://hz.yj202588.top/gtkfhrfmnq.html

esac
来源：http://hz.redwolf501.top/gtwrdrwmiv.html

[R12] for 遍历文件
来源：http://hz.yonumen.top/gtbizwaisv.html

for f in *.txt; do echo "$f"; done
来源：http://hz.chenlongwang.top/gtvirujgpo.html

[R13] for 计数循环
来源：http://hz.tanke756.top/gtwlqwodcg.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.xziqi.cn/gtjiyrvahp.html

[R14] C 风格 for
来源：http://hz.xingfuxueyuan.xyz/gtekncgwln.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.zycfv.cn/gtqolunghi.html

[R15] while 逐行读文件
来源：http://hz.52xcode.cn/gtivpjhvsq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.xylfe.cn/gthacqzakh.html

[R16] until 等待条件
来源：http://hz.jianghu66.top/gtxplpweip.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.gaohongyu789.top/gtwphfnhml.html

[R17] 数组定义与取值
来源：http://hz.sxryk.cn/gtbsxvzmye.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.guowangkeji.top/gtmctdwuqr.html

[R18] 遍历数组
来源：http://hz.shuidangran.top/gtprhazbhi.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.redwolf501.top/gteroaftqs.html

[R19] 数组长度
来源：http://hz.haohaochexian.top/gtmhmwhykt.html

echo "${#arr[@]}"
来源：http://hz.yangfankeji.com/gtbbrnixqw.html

[R20] 关联数组（字典）
来源：http://hz.shuidangran.top/gtwzqewdvh.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.havefunace.top/gtruhpolxm.html

[R21] 字符串长度
来源：http://hz.yvedp.cn/gtgtuthebj.html

echo "${#s}"
来源：http://hz.sweek.top/gtjogbhvua.html

[R22] 截取子串
来源：http://hz.hfpthk.cn/gtnqsohftm.html

echo "${s:0:5}"
来源：http://hz.hnqzz.top/gtfyryrgpo.html

[R23] 字符串替换
来源：http://hz.daria6918.cn/gttebocwjk.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.jinyuanbaomall.cn/gtewrfcrhk.html

[R24] 大小写转换
来源：http://hz.aibaodan.cn/gtqylavvmx.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.xuanzx.com/gthludhkbf.html

[R25] 去后缀 / 去前缀
来源：http://hz.andypj.xyz/gtflivpmyb.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.kuanghao11.cn/gtqftimcvw.html

[R26] 命令替换
来源：http://hz.xinyue.icu/gtcdwgoahd.html

now=$(date +%F); echo "$now"
来源：http://hz.hfpthk.cn/gtiibcyhky.html

[R27] 算术展开
来源：http://hz.yongpay.top/gtdujbpgxw.html

echo $((1 + 2 * 3))
来源：http://hz.sufxvd.cn/gtwnvtqsgp.html

[R28] 浮点运算
来源：http://hz.zhixingplan.top/gtnviptqbw.html

echo "scale=2; 10/3" | bc
来源：http://hz.jyoumei.cn/gtxynizibt.html

[R29] 定义函数
来源：http://hz.sysykeji.top/gtebrtdttp.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.daria6918.cn/gtqngurnwj.html

[R30] 函数返回状态码
来源：http://hz.yueranfly.top/gthhccdyyb.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.jyoumei.cn/gtoutpczaa.html

[R31] 局部变量
来源：http://hz.jinqigufen.top/gtstibebfp.html

f() { local x=1; echo "$x"; }
来源：http://hz.xylfe.cn/gtrdseavgf.html

[R32] 参数个数校验
来源：http://hz.tianlin.xyz/gtdgysdane.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.jlsjyb.cn/gtmbuyobnd.html

[R33] 捕获错误并提示行号
来源：http://hz.ppjwa.cn/gtlwjesoez.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.ivvv.top/gtpsyqiqij.html

[R34] 退出时清理
来源：http://hz.hammf.cn/gtixehyhde.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.yuxming.cn/gtduretoav.html

[R35] 后台执行并等待
来源：http://hz.gaohongyu789.top/gtubtskxzd.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.xingfuxueyuan.xyz/gtppvpfnkn.html

[R36] 并发执行多个任务
来源：http://hz.chenzaomai.com/gttoibputv.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.tanke756.top/gtyjjomikf.html

[R37] 把输出赋给变量
来源：http://hz.yj20258888.top/gttrsiebzy.html

files=$(ls -1)
来源：http://hz.hammf.cn/gthwteassl.html

[R38] 管道串联
来源：http://hz.0kj1m.cn/gtyhteoogo.html

cat a.txt | grep -i error | wc -l
来源：http://hz.cheryme.top/gtmsqhseeh.html

[R39] 重定向标准输出与错误
来源：http://hz.yueranfly.top/gtigkcrecg.html

cmd > out.log 2>&1
来源：http://hz.52xcode.cn/gtaqhmnpts.html

[R40] 追加写日志
来源：http://hz.pengpengdd.cyou/gtvnggrisj.html

echo "log" >> out.log
来源：http://hz.xylfe.cn/gtcctwroqy.html

[R41] 丢弃输出
来源：http://hz.gogol.net.cn/gtvrswpikq.html

cmd >/dev/null 2>&1
来源：http://hz.jiagoushi.top/gtussjgwgu.html

[R42] 输入重定向
来源：http://hz.quarkkingdee.top/gtdbttevtj.html

wc -l < a.txt
来源：http://hz.havefunace.top/gtwalzasql.html

[R43] 按名字查找文件
来源：http://hz.tian-w.cn/gtkvxyydhc.html

find . -name "*.log" -type f
来源：http://hz.316326.xyz/gtxtwfsadj.html

[R44] 按修改时间查找
来源：http://hz.yj20258888.top/gtevqvcgmp.html

find . -mtime -7 -type f
来源：http://hz.aizwys.cn/gthdxsbuux.html

[R45] 批量删除
来源：http://hz.yj20258888.top/gtrehathlf.html

find . -name "*.tmp" -delete
来源：http://hz.sysykeji.top/gtakhqtzwe.html

[R46] 递归替换文件内容
来源：http://hz.hywenlv.cn/gtmaulrxkw.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.shzxlz.cn/gtlecjusph.html

[R47] sed 单行替换
来源：http://hz.ydzc1.top/gtwymtstgb.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.vqdsnc.cn/gtltzhasng.html

[R48] awk 取指定列
来源：http://hz.gotoacloud.top/gteaaqjgjx.html

awk '{print $1, $3}' a.txt
来源：http://hz.redwolf501.top/gtvncprfdh.html

[R49] awk 带条件
来源：http://hz.ywan-chungtsiang.top/gtggdjdqnt.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.52xcode.cn/gtbsfcswrw.html

[R50] awk 求和
来源：http://hz.gogol.net.cn/gtusgvormp.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.iojbl.cn/gtiaqczasq.html

[R51] 排序去重取前几
来源：http://hz.hfpthk.cn/gtvpmsxdox.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.nanxinkj.top/gtyessmiuq.html

[R52] 统计行数
来源：http://hz.jinyuanbaomall.cn/gtzaxolmea.html

wc -l a.txt
来源：http://hz.jinqigufen.top/gtbbcttcdn.html

[R53] 查看文件头与实时尾
来源：http://hz.pengpengdd.cyou/gtuuhfdhqo.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.xziqi.cn/gtcptirzmt.html

[R54] 比较两个文件
来源：http://hz.316326.xyz/gtblxpizha.html

diff a.txt b.txt
来源：http://hz.zdqjudy.top/gtftxvqspr.html

[R55] 压缩与解压
来源：http://hz.sxryk.cn/gtyvozqfkh.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.chenlongwang.top/gtjhqfwrqk.html

[R56] 远程拷贝
来源：http://hz.wangdashe.top/gthmwnwbdh.html

scp file user@host:/path/
来源：http://hz.cqqwz.cn/gticrpzfio.html

[R57] 远程执行命令
来源：http://hz.yvedp.cn/gtxfxcdhbm.html

ssh user@host 'uptime'
来源：http://hz.cheryme.top/gtvsilvxcm.html

[R58] 下载文件
来源：http://hz.andypj.xyz/gtofgzyxoh.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.0kj1m.cn/gtvhwsliiv.html

[R59] 发 POST JSON
来源：http://hz.gogol.net.cn/gtujncwkjn.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.ydjk.org.cn/gtcvzmeath.html

[R60] 只看 HTTP 状态码
来源：http://hz.gzhubu.top/gthccqyvvb.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.yj20258888.top/gtgprrcrxj.html

[R61] 磁盘占用
来源：http://hz.jinqigufen.top/gtysnjkivs.html

df -h;  du -sh *
来源：http://hz.chenzaomai.com/gtsfqlwccx.html

[R62] 找最占空间的文件
来源：http://hz.cdnleiting.top/gtukjjjuag.html

du -ah . | sort -rh | head -10
来源：http://hz.hammf.cn/gtfxbvkrbi.html

[R63] 内存与进程
来源：http://hz.hywenlv.cn/gtsqhrfbkh.html

free -h;  ps aux | grep nginx
来源：http://hz.gzhubu.top/gtvggggrnl.html

[R64] 结束进程
来源：http://hz.quarkkingdee.top/gtribfixyr.html

kill -9 $(pgrep -f app.py)
来源：http://hz.jyoumei.cn/gtxkskcfdn.html

[R65] 查看端口占用
来源：http://hz.jianghu66.top/gtvouokvvx.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.guannengcc.top/gthsuaptrm.html

[R66] 定时任务
来源：http://hz.shzxlz.cn/gtnazuderi.html

crontab -e;  crontab -l
来源：http://hz.shanyushiyangkeji.top/gtsvarhnus.html

[R67] 生成随机十六进制串
来源：http://hz.tanke756.top/gtntzucort.html

openssl rand -hex 16
来源：http://hz.smart0.xyz/gtvlafguob.html

[R68] 计算文件校验值
来源：http://hz.dashuyun.cn/gtsglqgsvf.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.jianghu66.top/gtybjhvpti.html

[R69] 生成随机密码
来源：http://hz.cdnleiting.top/gtjpgzkorb.html

head -c 16 /dev/urandom | base64
来源：http://hz.sysykeji.top/gtvryuvbho.html

[R70] 时间戳与互转
来源：http://hz.ppjwa.cn/gtpubvzmeo.html

date +%s;  date -d @1700000000
来源：http://hz.chenjidiqi.icu/gtxanmycau.html

[R71] 日期格式化
来源：http://hz.chenjidiqi.icu/gtevbosflp.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.jinqigufen.top/gtmcsrzjlc.html

[R72] 等待端口就绪
来源：http://hz.gogol.net.cn/gtrnekrzzp.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.zhixingplan.top/gtyjhfywrt.html

[R73] 分割大日志
来源：http://hz.c1oappe.top/gthdlhbkfr.html

split -l 1000 big.log part_
来源：http://hz.meibo888.top/gthcrhdnby.html

[R74] 批量重命名
来源：http://hz.redwolf501.top/gtkstqzbbi.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.jqgufenzy.top/gtzcjwrzgk.html

[R75] 导出环境变量
来源：http://hz.zhoulong.xyz/gtpmcstcbp.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.gogol.net.cn/gtmrtnzqws.html

[R76] 使用临时文件
来源：http://hz.sysykeji.top/gtrhgohjbf.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.ybcxt.top/gttznarvqq.html

[R77] 读取用户输入
来源：http://hz.ehwqpu.com/gtvlkphwiu.html

read -rp "请输入: " ans
来源：http://hz.c1oappe.top/gtjycosqwb.html

[R78] 交互式菜单
来源：http://hz.xingfuxueyuan.xyz/gtftnbzboj.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.birdmap.top/gtjahrpqtr.html

[R79] 解析命令行选项
来源：http://hz.sysykeji.top/gtepsldymo.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.yangfankeji.com/gthjsqphfp.html

[R80] 查看脚本执行耗时
来源：http://hz.bjfxy.top/gttwjgmmez.html

time ./run.sh
来源：http://hz.aibaodan.cn/gtgipmlpph.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtiumnjwsd.html

S. C / C++ 专题
来源：http://hz.jinghuilouyu.cn/gtytvloaak.html

================================================================================
来源：http://hz.ivvv.top/gtsyufmqes.html

[S01] C：Hello World
来源：http://hz.hnqzz.top/gtxnbfnhky.html

#include <stdio.h>
来源：http://hz.jiagoushi.top/gtfouatkaz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.hnxiangtu.top/gtvnauzlxs.html

[S02] C：变量与格式化输出
来源：http://hz.nanxinkj.top/gtxeqoeeyx.html

int a = 10; printf("%d\n", a);
来源：http://hz.c1oappe.top/gtxvdnxswy.html

[S03] C：读入整数
来源：http://hz.birdmap.top/gtxhtkyyws.html

int x; scanf("%d", &x);
来源：http://hz.xinyue.icu/gtvlfxcytz.html

[S04] C：字符串复制
来源：http://hz.nanxinkj.top/gtptrpilda.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.xuanzx.com/gtqxfwstjh.html

[S05] C：字符串长度
来源：http://hz.xziqi.cn/gtotfpyccr.html

strlen(s)
来源：http://hz.tanke756.top/gtrzszpbyd.html

[S06] C：字符串比较
来源：http://hz.jinyuanbaomall.cn/gtfcwtufjf.html

strcmp(a, b) == 0
来源：http://hz.aibaodan.cn/gtlsjqiicn.html

[S07] C：数组遍历求和
来源：http://hz.shuidangran.top/gtnlplggvq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.dashuyun.cn/gtfqfqojdt.html

[S08] C：动态内存分配与释放
来源：http://hz.birdmap.top/gtxlnexcsn.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.yangfankeji.com/gtutyydyjs.html

[S09] C：结构体定义与初始化
来源：http://hz.hongshengwenyu.top/gtetscpbyk.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.guannengcc.top/gtgtnbhhke.html

[S10] C：指针与解引用
来源：http://hz.wangdashe.top/gtrhfugzkk.html

int *p = &a;  *p = 5;
来源：http://hz.yueranfly.top/gtrckhliid.html

[S11] C：逐行读文件
来源：http://hz.xuetiantiany.cn/gtdaqfbeks.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.jinyuanbaomall.cn/gtjnurxsti.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.tanke756.top/gtlxzpwfvq.html

fclose(f);
来源：http://hz.jiagoushi.top/gtqfvlhhls.html

[S12] C：写文件
来源：http://hz.quarkkingdee.top/gtnibcqjfv.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.quarkkingdee.top/gtqrrxxius.html

[S13] C：宏定义
来源：http://hz.yj20258.top/gthspepxlv.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.wangdashe.top/gtjccqwhes.html

[S14] C：枚举
来源：http://hz.dianchejie.cn/gtkwnrhflk.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.hongshengwenyu.top/gtljmynhoq.html

[S15] C：类型转换
来源：http://hz.redwolf501.top/gtdtxwiznu.html

(double) a / b
来源：http://hz.svipenyu.cn/gtoykvdfqj.html

[S16] C：位操作置位
来源：http://hz.iojbl.cn/gtfntxdwbx.html

x |= (1 << 3);
来源：http://hz.yuxming.cn/gtswlyqqfl.html

[S17] C：安全拼接字符串
来源：http://hz.andypj.xyz/gtgxelflis.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.wangdashe.top/gtuhbcveyd.html

[S18] C：命令行参数
来源：http://hz.bjfxy.top/gtpkzubeql.html

int main(int argc, char **argv)
来源：http://hz.shangyingyoupin.top/gtfrqewhtk.html

[S19] C：快速排序
来源：http://hz.hnqzz.top/gthvxkiobp.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.xinyue.icu/gtffxggqvh.html

[S20] C：二分查找
来源：http://hz.cucudq.cn/gtxhmgohid.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.iojbl.cn/gtdxanpucr.html

[S21] C：字符类别判断
来源：http://hz.hywenlv.cn/gtoancqfgv.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.zhijiandao.cn/gtmpanyykc.html

[S22] C：字符串转数字
来源：http://hz.zhengqikj.top/gtrsmcwsin.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.cucudq.cn/gtpoxldkhz.html

[S23] C：随机数
来源：http://hz.cqqwz.cn/gtdmmqyblt.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.yj202588.top/gtdblrsaeu.html

[S24] C：获取本地时间
来源：http://hz.havefunace.top/gtvifdftpj.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.pengpengdd.cyou/gtkowkdrrd.html

[S25] C：内存拷贝
来源：http://hz.hywenlv.cn/gtbjumdikl.html

memcpy(dst, src, n);
来源：http://hz.ppjwa.cn/gtilwusozw.html

[S26] C：内存清零
来源：http://hz.daxiang520.top/gtlrjuymoj.html

memset(a, 0, sizeof a);
来源：http://hz.tanke756.top/gtbtwcwjca.html

[S27] C：定义常量
来源：http://hz.meibo888.top/gtjdgvzkad.html

const double PI = 3.14159;
来源：http://hz.jyoumei.cn/gttzhfgaji.html

[S28] C：静态变量
来源：http://hz.hysaishi.cn/gtrrfttrwl.html

static int counter = 0;
来源：http://hz.0kj1m.cn/gtxuekpqgg.html

[S29] C：变参函数
来源：http://hz.tian-w.cn/gtqnrjimsb.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.yongpay.top/gtqfogslpg.html

[S30] C：头文件保护
来源：http://hz.zhiwuduotai.top/gtsfzupddn.html

#ifndef X_H
来源：http://hz.jyoumei.cn/gtvodywbmf.html

#define X_H
来源：http://hz.hnqzz.top/gtqsddruaq.html

#endif
来源：http://hz.hammf.cn/gtpigaanto.html

[S31] C++：Hello World
来源：http://hz.fzhhl.top/gtsvzjhsyx.html

#include <iostream>
来源：http://hz.yj20258888.top/gtpyxthgvd.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.vqdsnc.cn/gtxlgvzbfh.html

[S32] C++：字符串
来源：http://hz.yangfankeji.com/gtwpjilccy.html

std::string s = "hi";  s += "!";
来源：http://hz.gogol.net.cn/gtyqmbeklb.html

[S33] C++：vector 增删
来源：http://hz.zhijiandao.cn/gtmtlamgif.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.ydjk.org.cn/gthoopsqwu.html

[S34] C++：遍历 vector
来源：http://hz.9152youxi.cn/gtygumqoll.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.jinqigfzy.top/gtsppnjxwp.html

[S35] C++：map
来源：http://hz.snrcjt.cn/gtappxtfus.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.tianlin.xyz/gtwyjlmxwp.html

[S36] C++：unordered_map
来源：http://hz.jinyuanbaomall.cn/gtyaiwnyoc.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.ivvv.top/gtvcumgbaa.html

[S37] C++：set
来源：http://hz.yvedp.cn/gtpcfhplij.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.snrcjt.cn/gtxlqypned.html

[S38] C++：排序
来源：http://hz.daxiang520.top/gtcjjcfciv.html

std::sort(v.begin(), v.end());
来源：http://hz.316326.xyz/gtlbmjmssi.html


<!-- 参考信息 -->