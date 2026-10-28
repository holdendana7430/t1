代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.ydjk.org.cn/gtpqrufccp.html

[Q50] 批量更新
来源：http://hz.ehwqpu.com/gtytczrjfc.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.pycfn.com/gtkznzfdcb.html

[Q51] 用子查询更新
来源：http://hz.sysykeji.top/gtnvcpkmmf.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.bjfxy.top/gtbuiaiqmf.html

[Q52] 删除指定行
来源：http://hz.fengsongda.top/gtvbghhnda.html

DELETE FROM users WHERE id = 10;
来源：http://hz.pengpengdd.cyou/gtgibqzwne.html

[Q53] 按条件删除
来源：http://hz.shanyushiyangkeji.top/gtotqjnztq.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.hnxiangtu.top/gtokwtdpdf.html

[Q54] 清空表
来源：http://hz.sufxvd.cn/gtermeszaz.html

TRUNCATE TABLE logs;
来源：http://hz.shzxlz.cn/gtdiljhbcb.html

[Q55] 排名（并列占位）
来源：http://hz.shanyushiyangtech.top/gtwtpmjxsg.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.hfpthk.cn/gtbwxlcszn.html

[Q56] 密集排名（并列不占位）
来源：http://hz.hfpthk.cn/gtowszswtd.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.hywenlv.cn/gtoqbbozuc.html

[Q57] 行号
来源：http://hz.meibo888.top/gteykeiact.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.mhx1999.top/gtxfpdvlzf.html

[Q58] 累计求和
来源：http://hz.pengpengdd.cyou/gtvwahklpb.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.birdmap.top/gtyzkzsghe.html

[Q59] 分组内累计
来源：http://hz.quarkkingdee.top/gtgrczaofv.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.zdqjudy.top/gtebjbbvmn.html

[Q60] 取上一行 / 下一行
来源：http://hz.smart0.xyz/gtsopoedis.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.ywan-chungtsiang.top/gtpkcmqbcx.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.pycfn.com/gtjtklnmyj.html

[Q61] 移动平均
来源：http://hz.yj202588.top/gtfvhvwvjm.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.sufxvd.cn/gtqhipmeem.html

[Q62] 分组占比
来源：http://hz.shuidangran.top/gtmvoiuixp.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.shangyingyoupin.top/gtyyujoqrn.html

[Q63] 开启事务
来源：http://hz.ybcxt.top/gtrlffxtrx.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.vqdsnc.cn/gtezrrjpdv.html

[Q64] 提交事务
来源：http://hz.xylfe.cn/gtkxsqhkug.html

COMMIT;
来源：http://hz.daria6918.cn/gtrhsktrya.html

[Q65] 回滚事务
来源：http://hz.hnqzz.top/gttidtfwki.html

ROLLBACK;
来源：http://hz.zhongyouzk.top/gtqtwuovmc.html

[Q66] 行锁查询
来源：http://hz.cdnleiting.top/gtdqdroqeu.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.jinyuanbaomall.cn/gtimadxxhr.html

[Q67] 设置隔离级别
来源：http://hz.daria6918.cn/gtriyphuzz.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.cashguo.top/gtgechwuau.html

[Q68] 保存点
来源：http://hz.zhoulong.xyz/gtpfbnogrw.html

SAVEPOINT sp1;
来源：http://hz.sweek.top/gtimxxuwca.html

ROLLBACK TO sp1;
来源：http://hz.hnqzz.top/gtndqaaown.html

[Q69] 查看执行计划
来源：http://hz.svipenyu.cn/gtpzdfcwbb.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.aizwys.cn/gtwqapinrq.html

[Q70] 更新统计信息
来源：http://hz.cashguo.top/gtrrubfixb.html

ANALYZE TABLE users;
来源：http://hz.nanxuanxn.top/gtxxnqxtqu.html

[Q71] 查看建表语句
来源：http://hz.xingfuxueyuan.xyz/gtnfvsfiwy.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.smart0.xyz/gtrmwgefjb.html

[Q72] 查看索引
来源：http://hz.jinqigufen.top/gtwugihkvo.html

SHOW INDEX FROM users;
来源：http://hz.shanyushiyangkeji.top/gtcdcljlyt.html

[Q73] 查看表状态
来源：http://hz.shzxlz.cn/gtlrnridui.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.xinyue.icu/gtkzzrhupq.html

[Q74] 强制使用索引
来源：http://hz.jinyuanbaomall.cn/gtspeojkev.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.jqgfzy.top/gtaaydakki.html

[Q75] 日期格式化
来源：http://hz.havefunace.top/gtechtarjr.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.aizwys.cn/gtajmuykxy.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.vqdsnc.cn/gtbqizwvbs.html

[Q76] 按天统计
来源：http://hz.xylfe.cn/gtuhbzjmcv.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.shzxlz.cn/gttuuktjtd.html

[Q77] 时间加减
来源：http://hz.meibo888.top/gtbewvqqdp.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.ywan-chungtsiang.top/gteplrmgjp.html

[Q78] 当前时间
来源：http://hz.yvedp.cn/gtgsksgpuh.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.nanxuanxn.top/gtbzbjhlyo.html

[Q79] 字符串拼接
来源：http://hz.gogol.net.cn/gttfggqzvv.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.bjfxy.top/gtkirbkned.html

[Q80] 字符串截取
来源：http://hz.fengsongda.top/gtlyewvdde.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.ybcxt.top/gtxagucsyj.html

[Q81] 字符串替换
来源：http://hz.0kj1m.cn/gtcdltdshi.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.ehwqpu.com/gtwnvywujg.html

[Q82] 字符长度与字节长度
来源：http://hz.cqqwz.cn/gtuszpayit.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.jianghu66.top/gtecsquodc.html

[Q83] 大小写转换
来源：http://hz.ydzc1.top/gtzlxgupgy.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.guowangkeji.top/gttvgszbxd.html

[Q84] 去除首尾空格
来源：http://hz.gogol.net.cn/gtomrbyfcr.html

SELECT TRIM(name) FROM users;
来源：http://hz.kuanghao11.cn/gtpnjhsabg.html

[Q85] 数值取整
来源：http://hz.ywan-chungtsiang.top/gttvpdtghl.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.shanyushiyangkeji.top/gtnvnqtkpa.html

[Q86] 读取 JSON 字段
来源：http://hz.zhengqikj.top/gthuqlfigl.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.xylfe.cn/gtaujblsuo.html

[Q87] JSON 字段做条件
来源：http://hz.vqdsnc.cn/gtczpjtxvc.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.nanxinkj.top/gtfbjzfrei.html

[Q88] 行转列（条件聚合）
来源：http://hz.yj20258888.top/gtodeinelz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.xziqi.cn/gtsejoiajj.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.sysykeji.top/gtwacyzoqy.html

[Q89] 判断表是否存在
来源：http://hz.yj202588.top/gtgndfrsah.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.zhoulong.xyz/gtrwrdbwfb.html

[Q90] 生成序号列
来源：http://hz.pycfn.com/gtqsbnhqfd.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.yanxiufei.cn/gtkzswhmyk.html

================================================================================
来源：http://hz.sysykeji.top/gttzhwbidn.html

R. Bash 专题
来源：http://hz.hammf.cn/gtuvlnpgpz.html

================================================================================
来源：http://hz.haohaochexian.top/gtdijqvokm.html

[R01] shebang 与严格模式
来源：http://hz.redwolf501.top/gtlthysmil.html

#!/usr/bin/env bash
来源：http://hz.hnxiangtu.top/gtzwxmlnil.html

set -euo pipefail
来源：http://hz.iojbl.cn/gtqsyzskux.html

[R02] 变量赋值与使用
来源：http://hz.chenzaomai.com/gtfglqfdhn.html

name="Tom"; echo "$name"
来源：http://hz.hammf.cn/gtkapazkkq.html

[R03] 只读变量
来源：http://hz.yonumen.top/gtktlalnpi.html

readonly PI=3.14
来源：http://hz.nanxuanxn.top/gtpdzmucfb.html

[R04] 位置参数
来源：http://hz.smart0.xyz/gtnnyexoqf.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.havefunace.top/gtksdsidma.html

[R05] 参数默认值
来源：http://hz.ydjk.org.cn/gtswbwqyqn.html

name="${1:-default}"
来源：http://hz.xinyue.icu/gtdsohjbet.html

[R06] 判断命令是否存在
来源：http://hz.gaohongyu789.top/gtkhjctqez.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.fengsongda.top/gtsspmwykh.html

[R07] if 判断文件
来源：http://hz.fengsongda.top/gtlxsdbncv.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.meibo888.top/gtwolcelao.html

[R08] 数值比较
来源：http://hz.chenlongwang.top/gtlltcjmeq.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.fzhhl.top/gtvhljntje.html

[R09] 字符串比较
来源：http://hz.wangdashe.top/gtgruplrdd.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.sufxvd.cn/gtbaosorkk.html

[R10] 正则匹配
来源：http://hz.zhongyouzk.top/gtacqoaxgv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.ehwqpu.com/gtruyhzmup.html

[R11] case 多分支
来源：http://hz.jqgufenzy.top/gtsarpfcji.html

case "$1" in
来源：http://hz.yonumen.top/gtuonkxgoz.html

start) echo "启动" ;;
来源：http://hz.ivvv.top/gtklbgebgz.html

stop)  echo "停止" ;;
来源：http://hz.zhixingplan.top/gtostgvdnc.html

*)     echo "未知命令" ;;
来源：http://hz.ydzc1.top/gtvriprhae.html

esac
来源：http://hz.sufxvd.cn/gtdflikevu.html

[R12] for 遍历文件
来源：http://hz.zycfv.cn/gtunydbynm.html

for f in *.txt; do echo "$f"; done
来源：http://hz.ehwqpu.com/gtpbojvxpe.html

[R13] for 计数循环
来源：http://hz.pycfn.com/gtaggoasms.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.cqqwz.cn/gthojjgxrw.html

[R14] C 风格 for
来源：http://hz.jqgufenzy.top/gtvogddaym.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.wangdashe.top/gttfmuszhd.html

[R15] while 逐行读文件
来源：http://hz.9152youxi.cn/gtwjhhltaw.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.yueranfly.top/gtsktkvirg.html

[R16] until 等待条件
来源：http://hz.zhongyouzk.top/gtpisahxgl.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.xylfe.cn/gteyzamkft.html

[R17] 数组定义与取值
来源：http://hz.gaohongyu789.top/gtrcyhvoaz.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.hongshengwenyu.top/gtdkwcrccv.html

[R18] 遍历数组
来源：http://hz.zhongyouzk.top/gtqstdtpft.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.shanyushiyangkeji.top/gtjeziiagx.html

[R19] 数组长度
来源：http://hz.ivvv.top/gtwvdddqfs.html

echo "${#arr[@]}"
来源：http://hz.yj20258888.top/gtzougjerw.html

[R20] 关联数组（字典）
来源：http://hz.gogol.net.cn/gtgmtconza.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.yj202588.top/gtizekivwg.html

[R21] 字符串长度
来源：http://hz.zhixingplan.top/gtlpgmgxbu.html

echo "${#s}"
来源：http://hz.zhengqikj.top/gtvszcqzan.html

[R22] 截取子串
来源：http://hz.yj202588.top/gtbpqetqam.html

echo "${s:0:5}"
来源：http://hz.zycfv.cn/gtsqkdlaak.html

[R23] 字符串替换
来源：http://hz.xinyue.icu/gtasatcrth.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.havefunace.top/gtmjujbvbv.html

[R24] 大小写转换
来源：http://hz.cdnleiting.top/gtczerdhkh.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.jinqigufen.top/gtiiibfmqs.html

[R25] 去后缀 / 去前缀
来源：http://hz.wangshuangyany.cn/gtpmxjqrko.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.zdqjudy.top/gtocmkvtwk.html

[R26] 命令替换
来源：http://hz.havefunace.top/gtbptfuzsm.html

now=$(date +%F); echo "$now"
来源：http://hz.yonumen.top/gthzzanrws.html

[R27] 算术展开
来源：http://hz.zhoulong.xyz/gtszyogmjd.html

echo $((1 + 2 * 3))
来源：http://hz.shanyushiyangtech.top/gtnvtobxov.html

[R28] 浮点运算
来源：http://hz.meibo888.top/gtdksokhua.html

echo "scale=2; 10/3" | bc
来源：http://hz.jinyuanbaomall.cn/gtflnbmyfv.html

[R29] 定义函数
来源：http://hz.chenzaomai.com/gtjitnkppt.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.zhengqikj.top/gtyaqzfdzu.html

[R30] 函数返回状态码
来源：http://hz.shuidangran.top/gtfbguelcf.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.wangdashe.top/gtlxkwjicx.html

[R31] 局部变量
来源：http://hz.jiagoushi.top/gtzwvrmtiu.html

f() { local x=1; echo "$x"; }
来源：http://hz.iojbl.cn/gthnkpcveu.html

[R32] 参数个数校验
来源：http://hz.jianghu66.top/gtwupqtvwv.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.yanxiufei.cn/gtflmdmoqo.html

[R33] 捕获错误并提示行号
来源：http://hz.aibaodan.cn/gtmetvxbjn.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.hywenlv.cn/gtvcpffpsb.html

[R34] 退出时清理
来源：http://hz.tian-w.cn/gtcpdrotcj.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.xinyue.icu/gtwtieuyef.html

[R35] 后台执行并等待
来源：http://hz.tanke756.top/gtpopftisi.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.shangyingyoupin.top/gtiyyrwunx.html

[R36] 并发执行多个任务
来源：http://hz.snrcjt.cn/gtjvvszseo.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.pengpengdd.cyou/gtxmddlvni.html

[R37] 把输出赋给变量
来源：http://hz.jqgufenzy.top/gtvdnlkwef.html

files=$(ls -1)
来源：http://hz.fzhhl.top/gtcjgnwgnd.html

[R38] 管道串联
来源：http://hz.cqqwz.cn/gtvkngzfga.html

cat a.txt | grep -i error | wc -l
来源：http://hz.jqgufenzy.top/gtjmmrkdxd.html

[R39] 重定向标准输出与错误
来源：http://hz.ppjwa.cn/gtosuxwcnj.html

cmd > out.log 2>&1
来源：http://hz.mhx1999.top/gtvamduhps.html

[R40] 追加写日志
来源：http://hz.cdnleiting.top/gtjuuhrpfw.html

echo "log" >> out.log
来源：http://hz.hongshengwenyu.top/gtlmqctabh.html

[R41] 丢弃输出
来源：http://hz.c1oappe.top/gtlanohbta.html

cmd >/dev/null 2>&1
来源：http://hz.guowangkeji.top/gtoetyclcz.html

[R42] 输入重定向
来源：http://hz.yanxiufei.cn/gtjxxowjtr.html

wc -l < a.txt
来源：http://hz.hnqzz.top/gtguwjuwyv.html

[R43] 按名字查找文件
来源：http://hz.c1oappe.top/gthbqldzpt.html

find . -name "*.log" -type f
来源：http://hz.sysykeji.top/gtlsckojol.html

[R44] 按修改时间查找
来源：http://hz.nwbrower.top/gttwrzdrvq.html

find . -mtime -7 -type f
来源：http://hz.yanxiufei.cn/gtdhbhuqro.html

[R45] 批量删除
来源：http://hz.52xcode.cn/gthojwaewz.html

find . -name "*.tmp" -delete
来源：http://hz.zhaomingkeji.xyz/gtulhrsbno.html

[R46] 递归替换文件内容
来源：http://hz.zdqjudy.top/gtykxwmmje.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.daxiang520.top/gtcikfjqoa.html

[R47] sed 单行替换
来源：http://hz.nanxuanxn.top/gtjjbclupu.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.tian-w.cn/gtfpsockul.html

[R48] awk 取指定列
来源：http://hz.nwbrower.top/gtkevepxgq.html

awk '{print $1, $3}' a.txt
来源：http://hz.yongpay.top/gtirufjxkb.html

[R49] awk 带条件
来源：http://hz.316326.xyz/gtxbktkbgv.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.shanyushiyangtech.top/gtrruaryef.html

[R50] awk 求和
来源：http://hz.ivvv.top/gtasjacuza.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.bjfxy.top/gtvyxkvnhp.html

[R51] 排序去重取前几
来源：http://hz.jiagoushi.top/gtlzixnytm.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.xuetiantiany.cn/gttxoyebek.html

[R52] 统计行数
来源：http://hz.haohaochexian.top/gttnsbyser.html

wc -l a.txt
来源：http://hz.hongshengwenyu.top/gtthvwhtzm.html

[R53] 查看文件头与实时尾
来源：http://hz.nanxinkj.top/gtlrpmrprm.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.52xcode.cn/gtozsxmmim.html

[R54] 比较两个文件
来源：http://hz.yonumen.top/gtunkrehrc.html

diff a.txt b.txt
来源：http://hz.cashguo.top/gtgkcbwigs.html

[R55] 压缩与解压
来源：http://hz.zhongyouzk.top/gtgixkwxgl.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.cqqwz.cn/gtvjmvcddw.html

[R56] 远程拷贝
来源：http://hz.yuxming.cn/gtctgfbbei.html

scp file user@host:/path/
来源：http://hz.chenzaomai.com/gtmvisytfh.html

[R57] 远程执行命令
来源：http://hz.snrcjt.cn/gtiwrlyxnp.html

ssh user@host 'uptime'
来源：http://hz.wangshuangyany.cn/gtlvgpsrva.html

[R58] 下载文件
来源：http://hz.ybcxt.top/gtppogerat.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.hnxiangtu.top/gtooilzhhm.html

[R59] 发 POST JSON
来源：http://hz.chenzaomai.com/gtitpreuaa.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.kuanghao11.cn/gtdsaoggxv.html

[R60] 只看 HTTP 状态码
来源：http://hz.andypj.xyz/gthnuqxvka.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.guannengcc.top/gtdvjurhow.html

[R61] 磁盘占用
来源：http://hz.cucudq.cn/gtbdespape.html

df -h;  du -sh *
来源：http://hz.yuanzhike.top/gtdxkiwvae.html

[R62] 找最占空间的文件
来源：http://hz.cucudq.cn/gtjmtbwpea.html

du -ah . | sort -rh | head -10
来源：http://hz.hnxiangtu.top/gtkhupcedz.html

[R63] 内存与进程
来源：http://hz.zhiwuduotai.top/gtolbemeol.html

free -h;  ps aux | grep nginx
来源：http://hz.nanxuanxn.top/gtqkupnsqn.html

[R64] 结束进程
来源：http://hz.zhongyouzk.top/gtjrcbiwjm.html

kill -9 $(pgrep -f app.py)
来源：http://hz.dashuyun.cn/gtzocrooab.html

[R65] 查看端口占用
来源：http://hz.birdmap.top/gtgbsgyqqo.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.cheryme.top/gtzvkypqqy.html

[R66] 定时任务
来源：http://hz.shangyingyoupin.top/gtbeudzepv.html

crontab -e;  crontab -l
来源：http://hz.316326.xyz/gtprderrxo.html

[R67] 生成随机十六进制串
来源：http://hz.mhx1999.top/gtezsuijqu.html

openssl rand -hex 16
来源：http://hz.sxryk.cn/gtwleqgoty.html

[R68] 计算文件校验值
来源：http://hz.quarkkingdee.top/gtbbxaboxg.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.xingfuxueyuan.xyz/gtcnnfedox.html

[R69] 生成随机密码
来源：http://hz.chenlongwang.top/gttnotcpnv.html

head -c 16 /dev/urandom | base64
来源：http://hz.svipenyu.cn/gttfyoysxm.html

[R70] 时间戳与互转
来源：http://hz.yanxiufei.cn/gtruvrxedl.html

date +%s;  date -d @1700000000
来源：http://hz.yueranfly.top/gtdrwtnyow.html

[R71] 日期格式化
来源：http://hz.iojbl.cn/gtunawusia.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.cucudq.cn/gtyksuweal.html

[R72] 等待端口就绪
来源：http://hz.cashguo.top/gtxmwqxyge.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.svipenyu.cn/gttpswxfrz.html

[R73] 分割大日志
来源：http://hz.yuxming.cn/gtcrbsrzeq.html

split -l 1000 big.log part_
来源：http://hz.dianchejie.cn/gtazaxgztz.html

[R74] 批量重命名
来源：http://hz.svipenyu.cn/gtazqyqrdm.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.andypj.xyz/gtzrswwumb.html

[R75] 导出环境变量
来源：http://hz.hywenlv.cn/gteeuuthhe.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.quarkkingdee.top/gtwftdqzqb.html

[R76] 使用临时文件
来源：http://hz.gotoacloud.top/gtpcoaahjc.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.zhijiandao.cn/gtqwtiqhim.html

[R77] 读取用户输入
来源：http://hz.ehwqpu.com/gtaknginqy.html

read -rp "请输入: " ans
来源：http://hz.hywenlv.cn/gtxrlklnfu.html

[R78] 交互式菜单
来源：http://hz.ybcxt.top/gtregkafmm.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.wangdashe.top/gthbkfprvy.html

[R79] 解析命令行选项
来源：http://hz.dianchejie.cn/gtvorhmugz.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.jlsjyb.cn/gtfdrrwcip.html

[R80] 查看脚本执行耗时
来源：http://hz.wangshuangyany.cn/gtjsbgjngr.html

time ./run.sh
来源：http://hz.yuxming.cn/gtgisjabql.html

================================================================================
来源：http://hz.hammf.cn/gtokraxqic.html

S. C / C++ 专题
来源：http://hz.sxryk.cn/gtdpqgdjmi.html

================================================================================
来源：http://hz.cucudq.cn/gtbalmpbcu.html

[S01] C：Hello World
来源：http://hz.redwolf501.top/gtnqmyktsz.html

#include <stdio.h>
来源：http://hz.dashuyun.cn/gtwoqwztuo.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.gotoacloud.top/gttzrmrfxw.html

[S02] C：变量与格式化输出
来源：http://hz.cqqwz.cn/gtvbwcjswr.html

int a = 10; printf("%d\n", a);
来源：http://hz.bjfxy.top/gtijinvdbo.html

[S03] C：读入整数
来源：http://hz.svipenyu.cn/gtgugqjqty.html

int x; scanf("%d", &x);
来源：http://hz.yongpay.top/gtkrjqvtpu.html

[S04] C：字符串复制
来源：http://hz.quarkkingdee.top/gtxqsjufor.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.xinyue.icu/gttkypizwl.html

[S05] C：字符串长度
来源：http://hz.wangdashe.top/gtbbarssvs.html

strlen(s)
来源：http://hz.hfpthk.cn/gtvwxwsbuo.html

[S06] C：字符串比较
来源：http://hz.gaohongyu789.top/gthgemrhin.html

strcmp(a, b) == 0
来源：http://hz.meibo888.top/gthhnmsaaa.html

[S07] C：数组遍历求和
来源：http://hz.sysykeji.top/gtmygldvnz.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.cdnleiting.top/gtcvihgjez.html

[S08] C：动态内存分配与释放
来源：http://hz.xingfuxueyuan.xyz/gtojyodsoy.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.jianghu66.top/gteloethre.html

[S09] C：结构体定义与初始化
来源：http://hz.shzxlz.cn/gtcjltzcaz.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.fzhhl.top/gtsmnszdzs.html

[S10] C：指针与解引用
来源：http://hz.yj202588.top/gtsetwogbq.html

int *p = &a;  *p = 5;
来源：http://hz.tanke756.top/gtbfbamwkl.html

[S11] C：逐行读文件
来源：http://hz.aibaodan.cn/gtyijzxcos.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.9152youxi.cn/gtptwdcurp.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.nanxuanxn.top/gtdkizrcdj.html

fclose(f);
来源：http://hz.tanke756.top/gtahgcnkyy.html

[S12] C：写文件
来源：http://hz.cqqwz.cn/gtulgihvln.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.yueranfly.top/gtqijcoysy.html

[S13] C：宏定义
来源：http://hz.gzhubu.top/gtuzkcfsis.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.zhoulong.xyz/gtgnzxffpl.html

[S14] C：枚举
来源：http://hz.tanke756.top/gtzqbxgqnn.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.gogol.net.cn/gtszfjxygj.html

[S15] C：类型转换
来源：http://hz.jqgufenzy.top/gtjijciecc.html

(double) a / b
来源：http://hz.nwbrower.top/gtiwcjrtut.html

[S16] C：位操作置位
来源：http://hz.ydjk.org.cn/gtcvmxsrms.html

x |= (1 << 3);
来源：http://hz.birdmap.top/gtymbgwakb.html

[S17] C：安全拼接字符串
来源：http://hz.daxiang520.top/gtslixbjwl.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.jinghuilouyu.cn/gtownjfifu.html

[S18] C：命令行参数
来源：http://hz.nanxinkj.top/gtqglzchez.html

int main(int argc, char **argv)
来源：http://hz.hongshengwenyu.top/gtkwzqprnj.html

[S19] C：快速排序
来源：http://hz.wangdashe.top/gtujqhwztf.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.aizwys.cn/gtztyeekmb.html

[S20] C：二分查找
来源：http://hz.gotoacloud.top/gtktglqcxf.html


<!-- 参考信息 -->