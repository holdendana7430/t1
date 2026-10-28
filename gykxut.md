代发 wailian999

[Q67] 设置隔离级别
来源：http://hz.guowangkeji.top/gtkukdqvnq.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.nanxuanxn.top/gtiyhyrqcl.html

[Q68] 保存点
来源：http://hz.bjfxy.top/gtswxuoczb.html

SAVEPOINT sp1;
来源：http://hz.9152youxi.cn/gtwgfedrgu.html

ROLLBACK TO sp1;
来源：http://hz.dianchejie.cn/gtoxciseaj.html

[Q69] 查看执行计划
来源：http://hz.zdqjudy.top/gtdoiwghom.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.0kj1m.cn/gtxokrawia.html

[Q70] 更新统计信息
来源：http://hz.haohaochexian.top/gtyatmkibz.html

ANALYZE TABLE users;
来源：http://hz.cashguo.top/gtvovflqht.html

[Q71] 查看建表语句
来源：http://hz.dashuyun.cn/gtpqbxelci.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.shangyingyoupin.top/gtqgikzyrn.html

[Q72] 查看索引
来源：http://hz.zhongyouzk.top/gteyefuskm.html

SHOW INDEX FROM users;
来源：http://hz.cqqwz.cn/gtfuxnrjqv.html

[Q73] 查看表状态
来源：http://hz.chenjidiqi.icu/gtlrqucicc.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.gaohongyu789.top/gtuphtbocn.html

[Q74] 强制使用索引
来源：http://hz.zycfv.cn/gtoyevbdul.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.shzxlz.cn/gtghousnqj.html

[Q75] 日期格式化
来源：http://hz.jinqigufen.top/gtbuscscte.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.zdqjudy.top/gtmnnhuqno.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.xuetiantiany.cn/gtyyybrafk.html

[Q76] 按天统计
来源：http://hz.shuidangran.top/gtznwsedlc.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.snrcjt.cn/gtqxydibxj.html

[Q77] 时间加减
来源：http://hz.jinqigufen.top/gtsechaszw.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.gogol.net.cn/gtytsxmobd.html

[Q78] 当前时间
来源：http://hz.snrcjt.cn/gtskxbymbq.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.cdnleiting.top/gtddctdrtc.html

[Q79] 字符串拼接
来源：http://hz.chenlongwang.top/gtlzxoqfuj.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.aizwys.cn/gtuvqevpzt.html

[Q80] 字符串截取
来源：http://hz.chenjidiqi.icu/gtyuopjvqi.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.pengpengdd.cyou/gtsdyinrva.html

[Q81] 字符串替换
来源：http://hz.hnqzz.top/gtxrhcjbdd.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.nanxuanxn.top/gtliawouhv.html

[Q82] 字符长度与字节长度
来源：http://hz.wangdashe.top/gtnuxkmylz.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.zhongyouzk.top/gtrgnidevs.html

[Q83] 大小写转换
来源：http://hz.tianlin.xyz/gtsihspctj.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.jinqigfzy.top/gtboacaqzq.html

[Q84] 去除首尾空格
来源：http://hz.jinqigufen.top/gtiaqiuujg.html

SELECT TRIM(name) FROM users;
来源：http://hz.tanke756.top/gtzbirsdgi.html

[Q85] 数值取整
来源：http://hz.pengpengdd.cyou/gtpuwszjae.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.dashuyun.cn/gtxqrgpzha.html

[Q86] 读取 JSON 字段
来源：http://hz.cashguo.top/gtbusymhzt.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.chenlongwang.top/gthajvvdpj.html

[Q87] JSON 字段做条件
来源：http://hz.jinqigufen.top/gtremlkrqb.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.dashuyun.cn/gtcveilpkw.html

[Q88] 行转列（条件聚合）
来源：http://hz.shangyingyoupin.top/gtsswmpfwr.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.gzhubu.top/gtychsmgoo.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.tian-w.cn/gtynzzrpbb.html

[Q89] 判断表是否存在
来源：http://hz.yuxming.cn/gtmendmtvo.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.9152youxi.cn/gtmmvxyxvm.html

[Q90] 生成序号列
来源：http://hz.hfpthk.cn/gtdzdmsrnz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.xylfe.cn/gtkupiosju.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtsiixrpnp.html

R. Bash 专题
来源：http://hz.fzhhl.top/gtkzjofvir.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtaqeboklo.html

[R01] shebang 与严格模式
来源：http://hz.zhongyouzk.top/gtoitumiqq.html

#!/usr/bin/env bash
来源：http://hz.snrcjt.cn/gtladfgmls.html

set -euo pipefail
来源：http://hz.redwolf501.top/gtertklyrj.html

[R02] 变量赋值与使用
来源：http://hz.shzxlz.cn/gtbcckmqar.html

name="Tom"; echo "$name"
来源：http://hz.wangshuangyany.cn/gtjpxmxztl.html

[R03] 只读变量
来源：http://hz.yonumen.top/gtwpschrqy.html

readonly PI=3.14
来源：http://hz.zhengqikj.top/gtuuuncriz.html

[R04] 位置参数
来源：http://hz.yj20258.top/gtfuqzjrzd.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.hysaishi.cn/gtfvhtqdhg.html

[R05] 参数默认值
来源：http://hz.guowangkeji.top/gtviwnnmjr.html

name="${1:-default}"
来源：http://hz.bjfxy.top/gtdlbkqlzc.html

[R06] 判断命令是否存在
来源：http://hz.guannengcc.top/gtuwslxgof.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.ehwqpu.com/gtcybybvuv.html

[R07] if 判断文件
来源：http://hz.daxiang520.top/gtzamdjkpd.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.daxiang520.top/gtqwgaruak.html

[R08] 数值比较
来源：http://hz.jlsjyb.cn/gtdqcyiaoa.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.xuanzx.com/gtbkwbzmgz.html

[R09] 字符串比较
来源：http://hz.jqgufenzy.top/gtmzfkzzsw.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.hysaishi.cn/gtpueswsja.html

[R10] 正则匹配
来源：http://hz.smart0.xyz/gtrydakvnu.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.yongpay.top/gtrfjphwgj.html

[R11] case 多分支
来源：http://hz.sxryk.cn/gtqvuzvhcx.html

case "$1" in
来源：http://hz.jlsjyb.cn/gtfxvqyaqg.html

start) echo "启动" ;;
来源：http://hz.fzhhl.top/gthxyjxjai.html

stop)  echo "停止" ;;
来源：http://hz.nwbrower.top/gtsyoajumh.html

*)     echo "未知命令" ;;
来源：http://hz.hywenlv.cn/gtouovqwib.html

esac
来源：http://hz.hysaishi.cn/gtmvwawpkv.html

[R12] for 遍历文件
来源：http://hz.iojbl.cn/gtxprkdxmb.html

for f in *.txt; do echo "$f"; done
来源：http://hz.ydzc1.top/gtqtipmdxg.html

[R13] for 计数循环
来源：http://hz.jlsjyb.cn/gtreuxetoy.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.zhongyouzk.top/gtsdddilsd.html

[R14] C 风格 for
来源：http://hz.yanxiufei.cn/gtehndrvtz.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.nwbrower.top/gtfymkdspg.html

[R15] while 逐行读文件
来源：http://hz.cashguo.top/gtewerdmhz.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.ppjwa.cn/gtosmkwlfs.html

[R16] until 等待条件
来源：http://hz.yvedp.cn/gtoauzhozq.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.chenlongwang.top/gtuqgmfotv.html

[R17] 数组定义与取值
来源：http://hz.yuxming.cn/gtwdszjtrd.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.yj202588.top/gtqsbfrnia.html

[R18] 遍历数组
来源：http://hz.zdqjudy.top/gtojdolqgy.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.nanxuanxn.top/gttukpcxly.html

[R19] 数组长度
来源：http://hz.jqgfzy.top/gtsouseigr.html

echo "${#arr[@]}"
来源：http://hz.tanke756.top/gtssjhukyx.html

[R20] 关联数组（字典）
来源：http://hz.daxiang520.top/gtgubzwlpb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.jyoumei.cn/gtjetgksdo.html

[R21] 字符串长度
来源：http://hz.gogol.net.cn/gtspluizhl.html

echo "${#s}"
来源：http://hz.cheryme.top/gtvckusgtx.html

[R22] 截取子串
来源：http://hz.yonumen.top/gtunwmzvyk.html

echo "${s:0:5}"
来源：http://hz.sufxvd.cn/gtkjzfpqcy.html

[R23] 字符串替换
来源：http://hz.316326.xyz/gtvxzgihwu.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.jqgfzy.top/gtfojradrn.html

[R24] 大小写转换
来源：http://hz.ydjk.org.cn/gttdchuziy.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.hammf.cn/gtpsiigdoj.html

[R25] 去后缀 / 去前缀
来源：http://hz.pycfn.com/gtqzjumitt.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.birdmap.top/gtihyehxmt.html

[R26] 命令替换
来源：http://hz.yj20258888.top/gtukicywmr.html

now=$(date +%F); echo "$now"
来源：http://hz.9152youxi.cn/gtmozzhqjj.html

[R27] 算术展开
来源：http://hz.shanyushiyangkeji.top/gtommksutd.html

echo $((1 + 2 * 3))
来源：http://hz.shangyingyoupin.top/gteldqpfpl.html

[R28] 浮点运算
来源：http://hz.hongshengwenyu.top/gtafpvtjjo.html

echo "scale=2; 10/3" | bc
来源：http://hz.feifeiyinyue.top/gtfawyakku.html

[R29] 定义函数
来源：http://hz.cucudq.cn/gtbyswgryr.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.hywenlv.cn/gtxukqcdlb.html

[R30] 函数返回状态码
来源：http://hz.zhongyouzk.top/gtqvtkkbgk.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.yueranfly.top/gtlpcswlpd.html

[R31] 局部变量
来源：http://hz.dianchejie.cn/gtxeomgsfo.html

f() { local x=1; echo "$x"; }
来源：http://hz.316326.xyz/gtswuhsdlt.html

[R32] 参数个数校验
来源：http://hz.sysykeji.top/gtufrcaufu.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.daxiang520.top/gtelmcbnfu.html

[R33] 捕获错误并提示行号
来源：http://hz.0kj1m.cn/gtrdqordbe.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.dashuyun.cn/gtptefesnr.html

[R34] 退出时清理
来源：http://hz.dianchejie.cn/gtwxxuivak.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.yonumen.top/gthcwgapem.html

[R35] 后台执行并等待
来源：http://hz.yongpay.top/gttijcqeao.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.yongpay.top/gtmypvsoql.html

[R36] 并发执行多个任务
来源：http://hz.zdqjudy.top/gthhmznagn.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.chenjidiqi.icu/gtjczmunzb.html

[R37] 把输出赋给变量
来源：http://hz.pycfn.com/gtlpxfjbha.html

files=$(ls -1)
来源：http://hz.jinqigufen.top/gtievcgwnt.html

[R38] 管道串联
来源：http://hz.shangyingyoupin.top/gtrxodhcgz.html

cat a.txt | grep -i error | wc -l
来源：http://hz.birdmap.top/gtshdrtovt.html

[R39] 重定向标准输出与错误
来源：http://hz.yuxming.cn/gtsqcwpetb.html

cmd > out.log 2>&1
来源：http://hz.xingfuxueyuan.xyz/gtthdrckvc.html

[R40] 追加写日志
来源：http://hz.aibaodan.cn/gtslonhqnt.html

echo "log" >> out.log
来源：http://hz.quarkkingdee.top/gthdsnyzmu.html

[R41] 丢弃输出
来源：http://hz.yj20258888.top/gtutwkgaqm.html

cmd >/dev/null 2>&1
来源：http://hz.jqgufenzy.top/gtqioqjhoz.html

[R42] 输入重定向
来源：http://hz.yj20258888.top/gtfjatdvzi.html

wc -l < a.txt
来源：http://hz.aibaodan.cn/gtjgzhnwvn.html

[R43] 按名字查找文件
来源：http://hz.daxiang520.top/gtgtyuenes.html

find . -name "*.log" -type f
来源：http://hz.pycfn.com/gtdhswnpdy.html

[R44] 按修改时间查找
来源：http://hz.zhaomingkeji.xyz/gtlisdcomo.html

find . -mtime -7 -type f
来源：http://hz.yonumen.top/gtexidnkpn.html

[R45] 批量删除
来源：http://hz.hnxiangtu.top/gtirfawzxm.html

find . -name "*.tmp" -delete
来源：http://hz.sufxvd.cn/gtkdexijbt.html

[R46] 递归替换文件内容
来源：http://hz.ivvv.top/gtfmyoeohp.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.iojbl.cn/gtcgjkvluq.html

[R47] sed 单行替换
来源：http://hz.yj20258.top/gtrcdfjdcs.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.jqgufenzy.top/gtwvdwrgjc.html

[R48] awk 取指定列
来源：http://hz.cashguo.top/gtefefslag.html

awk '{print $1, $3}' a.txt
来源：http://hz.yueranfly.top/gtnkmejmiy.html

[R49] awk 带条件
来源：http://hz.jyoumei.cn/gttzpdslmk.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.daria6918.cn/gtrlncvsdl.html

[R50] awk 求和
来源：http://hz.sxryk.cn/gtuszleexj.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.wangdashe.top/gtyolfurpq.html

[R51] 排序去重取前几
来源：http://hz.zycfv.cn/gtejbvggus.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.yangfankeji.com/gtsijrrlft.html

[R52] 统计行数
来源：http://hz.smart0.xyz/gtmvovfbxh.html

wc -l a.txt
来源：http://hz.yangfankeji.com/gtmwayjwio.html

[R53] 查看文件头与实时尾
来源：http://hz.daria6918.cn/gtgnxtcigh.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.quarkkingdee.top/gtgxragsfg.html

[R54] 比较两个文件
来源：http://hz.ivvv.top/gtlskgkmnt.html

diff a.txt b.txt
来源：http://hz.chenjidiqi.icu/gtdulrzfjl.html

[R55] 压缩与解压
来源：http://hz.xuetiantiany.cn/gtspsvspje.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.tianlin.xyz/gtwamnhkkj.html

[R56] 远程拷贝
来源：http://hz.0kj1m.cn/gtrisfnckl.html

scp file user@host:/path/
来源：http://hz.guowangkeji.top/gtphvupuft.html

[R57] 远程执行命令
来源：http://hz.haohaochexian.top/gtvxsnqbhe.html

ssh user@host 'uptime'
来源：http://hz.daria6918.cn/gtetyjfmue.html

[R58] 下载文件
来源：http://hz.bjfxy.top/gtwzzstkwa.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.ydjk.org.cn/gtqwmhxuec.html

[R59] 发 POST JSON
来源：http://hz.yonumen.top/gtrkijxqpr.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.xuetiantiany.cn/gtgqxcjmml.html

[R60] 只看 HTTP 状态码
来源：http://hz.meibo888.top/gtvezfkoju.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.fengsongda.top/gtybjqqdpo.html

[R61] 磁盘占用
来源：http://hz.0kj1m.cn/gtutcwddgd.html

df -h;  du -sh *
来源：http://hz.hywenlv.cn/gtlxeeroto.html

[R62] 找最占空间的文件
来源：http://hz.wangdashe.top/gtjstxdoon.html

du -ah . | sort -rh | head -10
来源：http://hz.guannengcc.top/gtdkvbinmh.html

[R63] 内存与进程
来源：http://hz.zdqjudy.top/gtbyiiwfcj.html

free -h;  ps aux | grep nginx
来源：http://hz.hysaishi.cn/gtsdwpatjg.html

[R64] 结束进程
来源：http://hz.jianghu66.top/gtbzypqnio.html

kill -9 $(pgrep -f app.py)
来源：http://hz.yj20258.top/gtptgpczhq.html

[R65] 查看端口占用
来源：http://hz.hongshengwenyu.top/gtuzgfcpar.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.jyoumei.cn/gteikzdiip.html

[R66] 定时任务
来源：http://hz.havefunace.top/gtdcsihjct.html

crontab -e;  crontab -l
来源：http://hz.cucudq.cn/gtmleqbdhv.html

[R67] 生成随机十六进制串
来源：http://hz.dashuyun.cn/gtdcuubtwp.html

openssl rand -hex 16
来源：http://hz.jianghu66.top/gtdtirvhjl.html

[R68] 计算文件校验值
来源：http://hz.yonumen.top/gtrnwqjbwn.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.shangyingyoupin.top/gtnvvwujpl.html

[R69] 生成随机密码
来源：http://hz.jianghu66.top/gtvygexnvh.html

head -c 16 /dev/urandom | base64
来源：http://hz.gogol.net.cn/gtfzcxqfqa.html

[R70] 时间戳与互转
来源：http://hz.hammf.cn/gtydqcbtwh.html

date +%s;  date -d @1700000000
来源：http://hz.jqgufenzy.top/gtuiuyvame.html

[R71] 日期格式化
来源：http://hz.cashguo.top/gtldqzfwli.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.cucudq.cn/gtqvhbpavu.html

[R72] 等待端口就绪
来源：http://hz.hfpthk.cn/gtxtxgrxfk.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.ehwqpu.com/gteblgabqd.html

[R73] 分割大日志
来源：http://hz.haohaochexian.top/gtyhcgtkxp.html

split -l 1000 big.log part_
来源：http://hz.zdqjudy.top/gtshcmpxnb.html

[R74] 批量重命名
来源：http://hz.gzhubu.top/gtesptmwud.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.tianlin.xyz/gtljcfdowr.html

[R75] 导出环境变量
来源：http://hz.meibo888.top/gtqqutskqd.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.hongshengwenyu.top/gtikqgsjwi.html

[R76] 使用临时文件
来源：http://hz.shanyushiyangkeji.top/gtlltbhsjb.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.jianghu66.top/gtmhjuvrri.html

[R77] 读取用户输入
来源：http://hz.jinyuanbaomall.cn/gtotxipubv.html

read -rp "请输入: " ans
来源：http://hz.snrcjt.cn/gtqweibbus.html

[R78] 交互式菜单
来源：http://hz.nwbrower.top/gtdlojkgmu.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.yj20258888.top/gtedhmcszq.html

[R79] 解析命令行选项
来源：http://hz.xylfe.cn/gtginlqxlq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.feifeiyinyue.top/gttosnnwvw.html

[R80] 查看脚本执行耗时
来源：http://hz.cashguo.top/gtfzgqpymz.html

time ./run.sh
来源：http://hz.shuidangran.top/gtrtdqorrs.html

================================================================================
来源：http://hz.nanxinkj.top/gtjarpusqu.html

S. C / C++ 专题
来源：http://hz.xuetiantiany.cn/gtcmuiiolh.html

================================================================================
来源：http://hz.jianghu66.top/gtlasfgghu.html

[S01] C：Hello World
来源：http://hz.sufxvd.cn/gtbbsyfknb.html

#include <stdio.h>
来源：http://hz.daria6918.cn/gtyarylhmp.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.zhijiandao.cn/gtgutgkhxq.html

[S02] C：变量与格式化输出
来源：http://hz.shzxlz.cn/gtrhavpsdo.html

int a = 10; printf("%d\n", a);
来源：http://hz.smart0.xyz/gtgdrqtvvc.html

[S03] C：读入整数
来源：http://hz.dianchejie.cn/gtadyjcjzp.html

int x; scanf("%d", &x);
来源：http://hz.shanyushiyangtech.top/gtuiaanvad.html

[S04] C：字符串复制
来源：http://hz.jinyuanbaomall.cn/gtgpvgkinm.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.yj20258.top/gtqpssneyx.html

[S05] C：字符串长度
来源：http://hz.yonumen.top/gtvjhqpecw.html

strlen(s)
来源：http://hz.zhongyouzk.top/gtzovnayiw.html

[S06] C：字符串比较
来源：http://hz.hywenlv.cn/gtvwywbbkf.html

strcmp(a, b) == 0
来源：http://hz.ywan-chungtsiang.top/gtgaxxyulp.html

[S07] C：数组遍历求和
来源：http://hz.zycfv.cn/gtdduehrvy.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.aizwys.cn/gtqhhnrhqd.html

[S08] C：动态内存分配与释放
来源：http://hz.zhaomingkeji.xyz/gtmkvzeuli.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.aibaodan.cn/gtotlxbsza.html

[S09] C：结构体定义与初始化
来源：http://hz.fengsongda.top/gtemorikdv.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.yj20258.top/gtjrinkpts.html

[S10] C：指针与解引用
来源：http://hz.xylfe.cn/gtiykurmvd.html

int *p = &a;  *p = 5;
来源：http://hz.ydjk.org.cn/gtblmeauce.html

[S11] C：逐行读文件
来源：http://hz.yuxming.cn/gtnzytyrso.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.yvedp.cn/gtfhknqhee.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.wangdashe.top/gtpsebarhc.html

fclose(f);
来源：http://hz.xuanzx.com/gtdddelvar.html

[S12] C：写文件
来源：http://hz.yj202588.top/gtieerqmxb.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.yj20258888.top/gtqbgvnvby.html

[S13] C：宏定义
来源：http://hz.feifeiyinyue.top/gtjgfncmce.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.zhoulong.xyz/gtudcbudmv.html

[S14] C：枚举
来源：http://hz.shangyingyoupin.top/gtdrlvccbs.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.yueranfly.top/gtsqfvnxot.html

[S15] C：类型转换
来源：http://hz.bjfxy.top/gtzcrrzekb.html

(double) a / b
来源：http://hz.svipenyu.cn/gtolzwqzlw.html

[S16] C：位操作置位
来源：http://hz.ydzc1.top/gtxumzsekh.html

x |= (1 << 3);
来源：http://hz.jinghuilouyu.cn/gthewtcqjt.html

[S17] C：安全拼接字符串
来源：http://hz.gotoacloud.top/gthwpahhed.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.sysykeji.top/gtctlmtihn.html

[S18] C：命令行参数
来源：http://hz.jianghu66.top/gtzdgrtrjk.html

int main(int argc, char **argv)
来源：http://hz.shuidangran.top/gtlndkbpmb.html

[S19] C：快速排序
来源：http://hz.dashuyun.cn/gtzaulknys.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.gotoacloud.top/gtquizxptq.html

[S20] C：二分查找
来源：http://hz.wangdashe.top/gtprpnyqsn.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.feifeiyinyue.top/gtvlmojbmw.html

[S21] C：字符类别判断
来源：http://hz.dianchejie.cn/gtztolhjqu.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.316326.xyz/gtwssklvhk.html

[S22] C：字符串转数字
来源：http://hz.xziqi.cn/gtdmufbgtr.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.vqdsnc.cn/gtpthnhtqt.html

[S23] C：随机数
来源：http://hz.cqqwz.cn/gtwnckznmi.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.zhixingplan.top/gtbkrqtxjb.html

[S24] C：获取本地时间
来源：http://hz.gaohongyu789.top/gtbzvotqlm.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.fzhhl.top/gtqrgozsgt.html

[S25] C：内存拷贝
来源：http://hz.sufxvd.cn/gtmkjvtfok.html

memcpy(dst, src, n);
来源：http://hz.xuetiantiany.cn/gtefqbwzzi.html

[S26] C：内存清零
来源：http://hz.tianlin.xyz/gtycnhfqnj.html

memset(a, 0, sizeof a);
来源：http://hz.shzxlz.cn/gtpnrnpqld.html

[S27] C：定义常量
来源：http://hz.ydjk.org.cn/gtyktiuqgu.html

const double PI = 3.14159;
来源：http://hz.jinqigfzy.top/gteygglaaj.html

[S28] C：静态变量
来源：http://hz.dashuyun.cn/gtzymobepa.html

static int counter = 0;
来源：http://hz.meibo888.top/gtnfulexcw.html

[S29] C：变参函数
来源：http://hz.yvedp.cn/gtprcsgfdl.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.andypj.xyz/gthcmdhkbb.html

[S30] C：头文件保护
来源：http://hz.cdnleiting.top/gtotkrjcek.html

#ifndef X_H
来源：http://hz.gotoacloud.top/gtksuzgslj.html

#define X_H
来源：http://hz.ybcxt.top/gtdnnlyirn.html

#endif
来源：http://hz.ywan-chungtsiang.top/gtkyzwilug.html

[S31] C++：Hello World
来源：http://hz.jinyuanbaomall.cn/gtctjrfnoq.html

#include <iostream>
来源：http://hz.ywan-chungtsiang.top/gtzcyzdqii.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.yj20258.top/gtgnujuhgz.html

[S32] C++：字符串
来源：http://hz.xingfuxueyuan.xyz/gtbpqoswoy.html

std::string s = "hi";  s += "!";
来源：http://hz.hnxiangtu.top/gtqjfvaghc.html

[S33] C++：vector 增删
来源：http://hz.zhengqikj.top/gtqvcapayu.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.jqgfzy.top/gtkzlmzzav.html

[S34] C++：遍历 vector
来源：http://hz.shuidangran.top/gtufnowani.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.vqdsnc.cn/gtxwrfsjzy.html

[S35] C++：map
来源：http://hz.9152youxi.cn/gtwqszbkcv.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zhaomingkeji.xyz/gtzrcebakz.html

[S36] C++：unordered_map
来源：http://hz.yongpay.top/gtvzfgfcmo.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.xziqi.cn/gtdbgfqfrs.html


<!-- 参考信息 -->