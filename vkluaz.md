代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.zdqjudy.top/gtbnasklrh.html

[Q54] 清空表
来源：http://hz.shzxlz.cn/gtemnmcczg.html

TRUNCATE TABLE logs;
来源：http://hz.svipenyu.cn/gtoltngkgj.html

[Q55] 排名（并列占位）
来源：http://hz.xylfe.cn/gtphtoomkt.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.zycfv.cn/gtsdwtezbc.html

[Q56] 密集排名（并列不占位）
来源：http://hz.hysaishi.cn/gtcijsxfxf.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.pycfn.com/gtnvdcpqdz.html

[Q57] 行号
来源：http://hz.bjfxy.top/gtogiwjhcu.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.gotoacloud.top/gtybpogrlv.html

[Q58] 累计求和
来源：http://hz.c1oappe.top/gtdesqwncj.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.dianchejie.cn/gtepmilqcw.html

[Q59] 分组内累计
来源：http://hz.dashuyun.cn/gtthgyujmb.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.ydzc1.top/gthziuvnmp.html

[Q60] 取上一行 / 下一行
来源：http://hz.cqqwz.cn/gtgjabwtdc.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.cucudq.cn/gtthstunhj.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.jinqigufen.top/gtgfhgrbou.html

[Q61] 移动平均
来源：http://hz.ppjwa.cn/gtgrkmuwew.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.yvedp.cn/gtbgxavckb.html

[Q62] 分组占比
来源：http://hz.xylfe.cn/gtaurtukdd.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.ydzc1.top/gtuwznfkby.html

[Q63] 开启事务
来源：http://hz.bjfxy.top/gtchgtydmf.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.nanxuanxn.top/gtagzccdrb.html

[Q64] 提交事务
来源：http://hz.wangdashe.top/gtsefaribp.html

COMMIT;
来源：http://hz.pycfn.com/gtzuqfnrpe.html

[Q65] 回滚事务
来源：http://hz.hysaishi.cn/gtravqqelc.html

ROLLBACK;
来源：http://hz.guowangkeji.top/gtmicigkzq.html

[Q66] 行锁查询
来源：http://hz.sxryk.cn/gtzeqoyhwh.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.wangshuangyany.cn/gtqldgjlhv.html

[Q67] 设置隔离级别
来源：http://hz.hongshengwenyu.top/gtpfixjowt.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.redwolf501.top/gtrmtjtiel.html

[Q68] 保存点
来源：http://hz.gogol.net.cn/gtunprftcz.html

SAVEPOINT sp1;
来源：http://hz.gaohongyu789.top/gtxjrhsoxv.html

ROLLBACK TO sp1;
来源：http://hz.52xcode.cn/gtddtimppx.html

[Q69] 查看执行计划
来源：http://hz.jinghuilouyu.cn/gtemfvfpcr.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.9152youxi.cn/gtlyccxbwd.html

[Q70] 更新统计信息
来源：http://hz.hammf.cn/gtmxujpggp.html

ANALYZE TABLE users;
来源：http://hz.tanke756.top/gtrojkptin.html

[Q71] 查看建表语句
来源：http://hz.shuidangran.top/gttiujudip.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.havefunace.top/gtgkpqehnr.html

[Q72] 查看索引
来源：http://hz.guannengcc.top/gtwzupuvnv.html

SHOW INDEX FROM users;
来源：http://hz.ydjk.org.cn/gtdiqtvgfy.html

[Q73] 查看表状态
来源：http://hz.xziqi.cn/gtleadmpau.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.ywan-chungtsiang.top/gtehmexndc.html

[Q74] 强制使用索引
来源：http://hz.cucudq.cn/gtfazrbbxt.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.mhx1999.top/gtznlfrnan.html

[Q75] 日期格式化
来源：http://hz.kuanghao11.cn/gtywvaosxe.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.316326.xyz/gtglprswwl.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.daria6918.cn/gtijhlxuyv.html

[Q76] 按天统计
来源：http://hz.jlsjyb.cn/gtcjnkvtpk.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.jinghuilouyu.cn/gthccwubhr.html

[Q77] 时间加减
来源：http://hz.yangfankeji.com/gtyygfntth.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.sufxvd.cn/gttlvakczu.html

[Q78] 当前时间
来源：http://hz.yj20258.top/gtjtcxiwbu.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.meibo888.top/gtwkywyxgt.html

[Q79] 字符串拼接
来源：http://hz.fengsongda.top/gtqnljserm.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.wangdashe.top/gtmzzgapgz.html

[Q80] 字符串截取
来源：http://hz.dianchejie.cn/gtliquhexa.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.havefunace.top/gtsgfqodzi.html

[Q81] 字符串替换
来源：http://hz.fzhhl.top/gtzehytvfg.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.jyoumei.cn/gtendgwutm.html

[Q82] 字符长度与字节长度
来源：http://hz.yongpay.top/gtzalcqbja.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.yj20258.top/gtkthwcedd.html

[Q83] 大小写转换
来源：http://hz.feifeiyinyue.top/gtdllxaqlb.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.cucudq.cn/gtpwujschd.html

[Q84] 去除首尾空格
来源：http://hz.wangdashe.top/gtvfbldzxb.html

SELECT TRIM(name) FROM users;
来源：http://hz.ehwqpu.com/gtbsgjmrjj.html

[Q85] 数值取整
来源：http://hz.xuetiantiany.cn/gtappltaua.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.jinqigfzy.top/gtfmbcofhe.html

[Q86] 读取 JSON 字段
来源：http://hz.xuanzx.com/gtexiwsmsu.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.hnxiangtu.top/gtrfgjrhus.html

[Q87] JSON 字段做条件
来源：http://hz.jinghuilouyu.cn/gtqpuxnycs.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.bjfxy.top/gtdmryarhs.html

[Q88] 行转列（条件聚合）
来源：http://hz.yuanzhike.top/gtihprdxng.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.pengpengdd.cyou/gtedhnupee.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.0kj1m.cn/gtffztxumg.html

[Q89] 判断表是否存在
来源：http://hz.hongshengwenyu.top/gtojlpexyd.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.aizwys.cn/gtgsuvhivc.html

[Q90] 生成序号列
来源：http://hz.zhengqikj.top/gtvtrhdaym.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.daxiang520.top/gtvvfcbtky.html

================================================================================
来源：http://hz.nanxuanxn.top/gttlkvchqf.html

R. Bash 专题
来源：http://hz.fzhhl.top/gtspqcqgxa.html

================================================================================
来源：http://hz.aizwys.cn/gtlbcehqnd.html

[R01] shebang 与严格模式
来源：http://hz.gogol.net.cn/gtpjdedezo.html

#!/usr/bin/env bash
来源：http://hz.birdmap.top/gtnupaeuwg.html

set -euo pipefail
来源：http://hz.chenzaomai.com/gtwkkmpfvu.html

[R02] 变量赋值与使用
来源：http://hz.haohaochexian.top/gtlqzguszx.html

name="Tom"; echo "$name"
来源：http://hz.hongshengwenyu.top/gtlesnfgai.html

[R03] 只读变量
来源：http://hz.zhiwuduotai.top/gtypkcopbn.html

readonly PI=3.14
来源：http://hz.hammf.cn/gtfzdriuob.html

[R04] 位置参数
来源：http://hz.daxiang520.top/gtrfjbieht.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.yvedp.cn/gtsxbjsurl.html

[R05] 参数默认值
来源：http://hz.redwolf501.top/gtxnesmtez.html

name="${1:-default}"
来源：http://hz.daria6918.cn/gtfjhwmsjx.html

[R06] 判断命令是否存在
来源：http://hz.fzhhl.top/gtcaztlvdq.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.chenjidiqi.icu/gtowdkgxsd.html

[R07] if 判断文件
来源：http://hz.wangshuangyany.cn/gtelfdlwwb.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.xuanzx.com/gtbqobrsup.html

[R08] 数值比较
来源：http://hz.ivvv.top/gttxhjssmf.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.aibaodan.cn/gtwxpuotho.html

[R09] 字符串比较
来源：http://hz.c1oappe.top/gtkaaqwkyn.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.pengpengdd.cyou/gtmuzmrapt.html

[R10] 正则匹配
来源：http://hz.wangdashe.top/gtibuhidsr.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.gaohongyu789.top/gtxbjgvzcy.html

[R11] case 多分支
来源：http://hz.mhx1999.top/gtfcnbgcrv.html

case "$1" in
来源：http://hz.jqgfzy.top/gtecpeurwx.html

start) echo "启动" ;;
来源：http://hz.vqdsnc.cn/gtsxffyunb.html

stop)  echo "停止" ;;
来源：http://hz.hysaishi.cn/gtlqdgvmpc.html

*)     echo "未知命令" ;;
来源：http://hz.zhijiandao.cn/gtwwlnrgpb.html

esac
来源：http://hz.jinqigufen.top/gtgilqngbk.html

[R12] for 遍历文件
来源：http://hz.havefunace.top/gtzmzenrpy.html

for f in *.txt; do echo "$f"; done
来源：http://hz.ydzc1.top/gtseplsctu.html

[R13] for 计数循环
来源：http://hz.jinyuanbaomall.cn/gtafzxwmct.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.316326.xyz/gtryrhtggo.html

[R14] C 风格 for
来源：http://hz.ppjwa.cn/gtyatzogdj.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.quarkkingdee.top/gthgtjeyjx.html

[R15] while 逐行读文件
来源：http://hz.meibo888.top/gtiybcrjof.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.chenzaomai.com/gtvyqqjchv.html

[R16] until 等待条件
来源：http://hz.aibaodan.cn/gtfttpsihy.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.nanxinkj.top/gtggtxjhnd.html

[R17] 数组定义与取值
来源：http://hz.chenlongwang.top/gtiggognrv.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.tianlin.xyz/gtnbqpskjf.html

[R18] 遍历数组
来源：http://hz.vqdsnc.cn/gthpscjhsc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.jiagoushi.top/gtgxktrgoe.html

[R19] 数组长度
来源：http://hz.yj20258.top/gtgenkwibe.html

echo "${#arr[@]}"
来源：http://hz.yongpay.top/gtmgaagjgi.html

[R20] 关联数组（字典）
来源：http://hz.jqgufenzy.top/gthrqzwnth.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.tanke756.top/gtblyxuamg.html

[R21] 字符串长度
来源：http://hz.ehwqpu.com/gtvhsfjgan.html

echo "${#s}"
来源：http://hz.nanxuanxn.top/gtmfzrwqnu.html

[R22] 截取子串
来源：http://hz.ppjwa.cn/gtiqcsoyuf.html

echo "${s:0:5}"
来源：http://hz.cucudq.cn/gtrmoxmwip.html

[R23] 字符串替换
来源：http://hz.gogol.net.cn/gtzrrsjwda.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.xuetiantiany.cn/gtexexlvir.html

[R24] 大小写转换
来源：http://hz.shangyingyoupin.top/gttosgzgrm.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.meibo888.top/gtewshsshw.html

[R25] 去后缀 / 去前缀
来源：http://hz.yonumen.top/gtmtoabysp.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.cqqwz.cn/gtroikjrik.html

[R26] 命令替换
来源：http://hz.dianchejie.cn/gtlkkzpvgs.html

now=$(date +%F); echo "$now"
来源：http://hz.jianghu66.top/gtjnvmvoyj.html

[R27] 算术展开
来源：http://hz.ybcxt.top/gtslcopkej.html

echo $((1 + 2 * 3))
来源：http://hz.mhx1999.top/gtykusyetj.html

[R28] 浮点运算
来源：http://hz.dianchejie.cn/gtxvmtjuqe.html

echo "scale=2; 10/3" | bc
来源：http://hz.kuanghao11.cn/gtzkmmkyyc.html

[R29] 定义函数
来源：http://hz.hnqzz.top/gtpbpuvaly.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.hysaishi.cn/gtvznterch.html

[R30] 函数返回状态码
来源：http://hz.meibo888.top/gtsynbiifv.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.hongshengwenyu.top/gtvpkkdrqm.html

[R31] 局部变量
来源：http://hz.hysaishi.cn/gtqkutpvis.html

f() { local x=1; echo "$x"; }
来源：http://hz.jqgufenzy.top/gtowstktkt.html

[R32] 参数个数校验
来源：http://hz.hysaishi.cn/gtrfqemuiw.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.gotoacloud.top/gtewicrbdb.html

[R33] 捕获错误并提示行号
来源：http://hz.pengpengdd.cyou/gthfpmlfqx.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.hongshengwenyu.top/gtnasmkhzy.html

[R34] 退出时清理
来源：http://hz.yuxming.cn/gtaznhhqeh.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.cqqwz.cn/gtquiaovgg.html

[R35] 后台执行并等待
来源：http://hz.kuanghao11.cn/gtqgsrgdtd.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.feifeiyinyue.top/gtbwsapfny.html

[R36] 并发执行多个任务
来源：http://hz.redwolf501.top/gtmoktsekv.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.vqdsnc.cn/gtcdxvyzej.html

[R37] 把输出赋给变量
来源：http://hz.shanyushiyangkeji.top/gtdlarzhxh.html

files=$(ls -1)
来源：http://hz.aizwys.cn/gtkocykjqu.html

[R38] 管道串联
来源：http://hz.shzxlz.cn/gtjfhhsywi.html

cat a.txt | grep -i error | wc -l
来源：http://hz.jqgfzy.top/gtbxuqwzrk.html

[R39] 重定向标准输出与错误
来源：http://hz.meibo888.top/gtzbbktmbn.html

cmd > out.log 2>&1
来源：http://hz.9152youxi.cn/gtdksyagis.html

[R40] 追加写日志
来源：http://hz.hammf.cn/gtuyhueode.html

echo "log" >> out.log
来源：http://hz.zhijiandao.cn/gtrnxhhtie.html

[R41] 丢弃输出
来源：http://hz.guannengcc.top/gtquryrgrv.html

cmd >/dev/null 2>&1
来源：http://hz.c1oappe.top/gtuysdttgi.html

[R42] 输入重定向
来源：http://hz.svipenyu.cn/gtxehjnmdd.html

wc -l < a.txt
来源：http://hz.ppjwa.cn/gtsrduxheo.html

[R43] 按名字查找文件
来源：http://hz.jinghuilouyu.cn/gtqbnnfjjd.html

find . -name "*.log" -type f
来源：http://hz.guowangkeji.top/gtnpfyhksj.html

[R44] 按修改时间查找
来源：http://hz.haohaochexian.top/gtkkulbqmp.html

find . -mtime -7 -type f
来源：http://hz.shanyushiyangtech.top/gtmafnverp.html

[R45] 批量删除
来源：http://hz.zhaomingkeji.xyz/gtkwdyhtzc.html

find . -name "*.tmp" -delete
来源：http://hz.guowangkeji.top/gtdtqxbvey.html

[R46] 递归替换文件内容
来源：http://hz.tanke756.top/gtjoejdhvk.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.daria6918.cn/gtxwaskrfo.html

[R47] sed 单行替换
来源：http://hz.ydjk.org.cn/gtoxufhmrn.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.fengsongda.top/gtgbajfldi.html

[R48] awk 取指定列
来源：http://hz.ydjk.org.cn/gtgjyjrxvt.html

awk '{print $1, $3}' a.txt
来源：http://hz.nwbrower.top/gtmdugkrjp.html

[R49] awk 带条件
来源：http://hz.chenjidiqi.icu/gtweflfkzb.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.sxryk.cn/gtdlsombor.html

[R50] awk 求和
来源：http://hz.xziqi.cn/gtjelhzmno.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.snrcjt.cn/gtxosfehbo.html

[R51] 排序去重取前几
来源：http://hz.feifeiyinyue.top/gtvsenjcuc.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.mhx1999.top/gtucbikeny.html

[R52] 统计行数
来源：http://hz.0kj1m.cn/gtqmxhuegu.html

wc -l a.txt
来源：http://hz.xziqi.cn/gtssgunwbs.html

[R53] 查看文件头与实时尾
来源：http://hz.ivvv.top/gtzoeohllj.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.c1oappe.top/gtlgydzbwh.html

[R54] 比较两个文件
来源：http://hz.feifeiyinyue.top/gtboxusqlm.html

diff a.txt b.txt
来源：http://hz.haohaochexian.top/gtodggkwxv.html

[R55] 压缩与解压
来源：http://hz.zhengqikj.top/gtrntxcosl.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.cashguo.top/gthqwaikdw.html

[R56] 远程拷贝
来源：http://hz.nwbrower.top/gtvbymtynp.html

scp file user@host:/path/
来源：http://hz.hongshengwenyu.top/gtlgaxeors.html

[R57] 远程执行命令
来源：http://hz.yanxiufei.cn/gtixkdnvts.html

ssh user@host 'uptime'
来源：http://hz.316326.xyz/gtaraaqlsi.html

[R58] 下载文件
来源：http://hz.ehwqpu.com/gtnogodygm.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.zhixingplan.top/gtbbljianb.html

[R59] 发 POST JSON
来源：http://hz.jinyuanbaomall.cn/gtenecdnix.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.kuanghao11.cn/gtiziruuba.html

[R60] 只看 HTTP 状态码
来源：http://hz.hnqzz.top/gtmltxlybs.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.nwbrower.top/gtbqwvxsba.html

[R61] 磁盘占用
来源：http://hz.sysykeji.top/gtdipjagkl.html

df -h;  du -sh *
来源：http://hz.daxiang520.top/gtqsdqqkwo.html

[R62] 找最占空间的文件
来源：http://hz.hnxiangtu.top/gtnbuglhna.html

du -ah . | sort -rh | head -10
来源：http://hz.tanke756.top/gtkvlprkbp.html

[R63] 内存与进程
来源：http://hz.yangfankeji.com/gtrbihjkxk.html

free -h;  ps aux | grep nginx
来源：http://hz.shanyushiyangtech.top/gtsbsaxcjk.html

[R64] 结束进程
来源：http://hz.dashuyun.cn/gtcqshvbjr.html

kill -9 $(pgrep -f app.py)
来源：http://hz.zhixingplan.top/gtpecqrfhj.html

[R65] 查看端口占用
来源：http://hz.xylfe.cn/gtlylngcao.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.ywan-chungtsiang.top/gtuyeavsgj.html

[R66] 定时任务
来源：http://hz.hywenlv.cn/gtwtpbxzkf.html

crontab -e;  crontab -l
来源：http://hz.cheryme.top/gtwthnucge.html

[R67] 生成随机十六进制串
来源：http://hz.nanxuanxn.top/gtnwlohvti.html

openssl rand -hex 16
来源：http://hz.hongshengwenyu.top/gtxvatluji.html

[R68] 计算文件校验值
来源：http://hz.wangdashe.top/gtapwhahcg.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.xinyue.icu/gtjceypihp.html

[R69] 生成随机密码
来源：http://hz.shanyushiyangkeji.top/gtpjwkpiog.html

head -c 16 /dev/urandom | base64
来源：http://hz.bjfxy.top/gtyvvnrbjs.html

[R70] 时间戳与互转
来源：http://hz.hysaishi.cn/gtjcbzxocf.html

date +%s;  date -d @1700000000
来源：http://hz.chenlongwang.top/gtfqptszdo.html

[R71] 日期格式化
来源：http://hz.jqgfzy.top/gtnnuauwsk.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.fengsongda.top/gtdooqdwex.html

[R72] 等待端口就绪
来源：http://hz.wangdashe.top/gtcgmyunue.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.sufxvd.cn/gtexvxhmbi.html

[R73] 分割大日志
来源：http://hz.nwbrower.top/gtuvcfaviu.html

split -l 1000 big.log part_
来源：http://hz.meibo888.top/gtdfdtezva.html

[R74] 批量重命名
来源：http://hz.jinqigufen.top/gtokksutrf.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.yvedp.cn/gtimnyjfgo.html

[R75] 导出环境变量
来源：http://hz.chenzaomai.com/gtrrriqydy.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.shanyushiyangkeji.top/gtbkbvtyab.html

[R76] 使用临时文件
来源：http://hz.316326.xyz/gtsyffusdi.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.sweek.top/gtlzwgvjpr.html

[R77] 读取用户输入
来源：http://hz.aibaodan.cn/gtmgxcieeb.html

read -rp "请输入: " ans
来源：http://hz.yj20258888.top/gthvxzsxbp.html

[R78] 交互式菜单
来源：http://hz.pengpengdd.cyou/gtjeibjegd.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.sysykeji.top/gtvqreahmc.html

[R79] 解析命令行选项
来源：http://hz.nwbrower.top/gtcavmccef.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.meibo888.top/gtettkrvwi.html

[R80] 查看脚本执行耗时
来源：http://hz.nwbrower.top/gtyitokpdh.html

time ./run.sh
来源：http://hz.sufxvd.cn/gtjajealpy.html

================================================================================
来源：http://hz.shzxlz.cn/gthrkyyzld.html

S. C / C++ 专题
来源：http://hz.yuanzhike.top/gtwiucebgt.html

================================================================================
来源：http://hz.hnxiangtu.top/gtnnjtrbbu.html

[S01] C：Hello World
来源：http://hz.gotoacloud.top/gtmbebwyle.html

#include <stdio.h>
来源：http://hz.xuanzx.com/gtfaqarlen.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.fengsongda.top/gtsunbbwys.html

[S02] C：变量与格式化输出
来源：http://hz.xingfuxueyuan.xyz/gtdcenegwk.html

int a = 10; printf("%d\n", a);
来源：http://hz.yuxming.cn/gtgcaiymtn.html

[S03] C：读入整数
来源：http://hz.daria6918.cn/gtwlmvcdjk.html

int x; scanf("%d", &x);
来源：http://hz.iojbl.cn/gtwikjtukh.html

[S04] C：字符串复制
来源：http://hz.zhijiandao.cn/gtfhkprikm.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.yj20258888.top/gtrxiyjcqj.html

[S05] C：字符串长度
来源：http://hz.shzxlz.cn/gtbbvcawdf.html

strlen(s)
来源：http://hz.hysaishi.cn/gtsqrjifzl.html

[S06] C：字符串比较
来源：http://hz.daria6918.cn/gtfevtxtpc.html

strcmp(a, b) == 0
来源：http://hz.snrcjt.cn/gtqzjuhpvs.html

[S07] C：数组遍历求和
来源：http://hz.wangshuangyany.cn/gtnkmywhbk.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.zhengqikj.top/gtisayehsd.html

[S08] C：动态内存分配与释放
来源：http://hz.cucudq.cn/gtixtnwwbe.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.yonumen.top/gtqazpnncp.html

[S09] C：结构体定义与初始化
来源：http://hz.xuetiantiany.cn/gtkbfxkyjf.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.pycfn.com/gtgerynglk.html

[S10] C：指针与解引用
来源：http://hz.shanyushiyangtech.top/gtwnbdqaxg.html

int *p = &a;  *p = 5;
来源：http://hz.chenzaomai.com/gtjjsmhfln.html

[S11] C：逐行读文件
来源：http://hz.yj202588.top/gtbsovkjha.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.wangdashe.top/gtbbxhmzvb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.tian-w.cn/gthbckfihl.html

fclose(f);
来源：http://hz.shuidangran.top/gtdglswprx.html

[S12] C：写文件
来源：http://hz.tian-w.cn/gtadcfxcjy.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.jyoumei.cn/gtpuanvoar.html

[S13] C：宏定义
来源：http://hz.jyoumei.cn/gtnnxxnbsb.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.c1oappe.top/gtdhigvlso.html

[S14] C：枚举
来源：http://hz.chenzaomai.com/gtrsbibazm.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.hnxiangtu.top/gtrowdcctz.html

[S15] C：类型转换
来源：http://hz.xziqi.cn/gtapoklxzj.html

(double) a / b
来源：http://hz.yueranfly.top/gtraysjytm.html

[S16] C：位操作置位
来源：http://hz.hnqzz.top/gtacyprdli.html

x |= (1 << 3);
来源：http://hz.yvedp.cn/gtffkhjmdm.html

[S17] C：安全拼接字符串
来源：http://hz.dianchejie.cn/gtsqttzmme.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.hfpthk.cn/gtelgclhym.html

[S18] C：命令行参数
来源：http://hz.shanyushiyangkeji.top/gtenncfypp.html

int main(int argc, char **argv)
来源：http://hz.vqdsnc.cn/gtmznqhckp.html

[S19] C：快速排序
来源：http://hz.wangdashe.top/gtogceipol.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.zhiwuduotai.top/gtsplmzaey.html

[S20] C：二分查找
来源：http://hz.aibaodan.cn/gtpuzzrtje.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.hammf.cn/gtfvkjuceg.html

[S21] C：字符类别判断
来源：http://hz.dashuyun.cn/gtxmcmboub.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.gzhubu.top/gtzhcigyqh.html

[S22] C：字符串转数字
来源：http://hz.smart0.xyz/gtxmyreryb.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.feifeiyinyue.top/gtavqugbjl.html

[S23] C：随机数
来源：http://hz.hnqzz.top/gtenhbiffd.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.daria6918.cn/gtarnqlana.html

[S24] C：获取本地时间
来源：http://hz.jinyuanbaomall.cn/gticyjbypj.html


<!-- 参考信息 -->