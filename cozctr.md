代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.xuetiantiany.cn/gtkgwwvffy.html

[Q52] 删除指定行
来源：http://hz.guowangkeji.top/gtpaqvdqxm.html

DELETE FROM users WHERE id = 10;
来源：http://hz.zhoulong.xyz/gtwmlklffz.html

[Q53] 按条件删除
来源：http://hz.zhijiandao.cn/gtsgohhrnt.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.shangyingyoupin.top/gtcbmccfar.html

[Q54] 清空表
来源：http://hz.yonumen.top/gtkqqtkbos.html

TRUNCATE TABLE logs;
来源：http://hz.yuxming.cn/gtvovhvqwt.html

[Q55] 排名（并列占位）
来源：http://hz.jqgfzy.top/gtpmjtvare.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.kuanghao11.cn/gtlbmmuojr.html

[Q56] 密集排名（并列不占位）
来源：http://hz.guannengcc.top/gtegoqpdmr.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.feifeiyinyue.top/gtluhdxfvl.html

[Q57] 行号
来源：http://hz.meibo888.top/gtevifrxjv.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.zycfv.cn/gtwyvfrlkd.html

[Q58] 累计求和
来源：http://hz.jqgfzy.top/gtsanftupc.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.ybcxt.top/gtecybbipr.html

[Q59] 分组内累计
来源：http://hz.jlsjyb.cn/gtaausbujy.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.feifeiyinyue.top/gtkpdomsod.html

[Q60] 取上一行 / 下一行
来源：http://hz.shangyingyoupin.top/gtwmjrvljs.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.wangshuangyany.cn/gtletfucyi.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.jinqigfzy.top/gtqyacwqle.html

[Q61] 移动平均
来源：http://hz.zhijiandao.cn/gthopwwwaq.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.svipenyu.cn/gtsvxqonid.html

[Q62] 分组占比
来源：http://hz.ehwqpu.com/gtvhrzurrp.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.jinyuanbaomall.cn/gtvxylsjtj.html

[Q63] 开启事务
来源：http://hz.wangshuangyany.cn/gtfwdfzgwb.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.snrcjt.cn/gtnmcdjqee.html

[Q64] 提交事务
来源：http://hz.xingfuxueyuan.xyz/gtjhyyeicg.html

COMMIT;
来源：http://hz.316326.xyz/gterzzwltx.html

[Q65] 回滚事务
来源：http://hz.iojbl.cn/gtysihzmin.html

ROLLBACK;
来源：http://hz.zhoulong.xyz/gtnjkeipry.html

[Q66] 行锁查询
来源：http://hz.jinghuilouyu.cn/gtotjaoakq.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.sufxvd.cn/gthwsqbvec.html

[Q67] 设置隔离级别
来源：http://hz.vqdsnc.cn/gtgtkcuchy.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.jqgfzy.top/gtmlwjmptj.html

[Q68] 保存点
来源：http://hz.hongshengwenyu.top/gtoygkflel.html

SAVEPOINT sp1;
来源：http://hz.jqgufenzy.top/gtslicowgl.html

ROLLBACK TO sp1;
来源：http://hz.chenlongwang.top/gtthsyydnr.html

[Q69] 查看执行计划
来源：http://hz.yueranfly.top/gtnxovjvrc.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.meibo888.top/gtdxiegylt.html

[Q70] 更新统计信息
来源：http://hz.tanke756.top/gtbflxwlbt.html

ANALYZE TABLE users;
来源：http://hz.sysykeji.top/gtdixbwesa.html

[Q71] 查看建表语句
来源：http://hz.ydjk.org.cn/gtknmaxrls.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.hnxiangtu.top/gtxpchjorv.html

[Q72] 查看索引
来源：http://hz.shuidangran.top/gtrhoclzli.html

SHOW INDEX FROM users;
来源：http://hz.xuetiantiany.cn/gtgcqkjikp.html

[Q73] 查看表状态
来源：http://hz.daxiang520.top/gtwmyzxiwc.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.shangyingyoupin.top/gtdellymvs.html

[Q74] 强制使用索引
来源：http://hz.aizwys.cn/gtkomkiurx.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.nwbrower.top/gtkinudfqv.html

[Q75] 日期格式化
来源：http://hz.shanyushiyangkeji.top/gtxfgwxppd.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.xinyue.icu/gtqoviyigy.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.aibaodan.cn/gtlfixjqkh.html

[Q76] 按天统计
来源：http://hz.zycfv.cn/gtxgtsqszs.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.smart0.xyz/gtnfhmmnmd.html

[Q77] 时间加减
来源：http://hz.zhiwuduotai.top/gtdghvqfnh.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.tianlin.xyz/gtudavkdle.html

[Q78] 当前时间
来源：http://hz.sxryk.cn/gtnrfltjut.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.jiagoushi.top/gtnzbbpdhg.html

[Q79] 字符串拼接
来源：http://hz.mhx1999.top/gtpvhyrhep.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.fzhhl.top/gtmxqjjzbh.html

[Q80] 字符串截取
来源：http://hz.smart0.xyz/gtpsfdbcmf.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.jqgufenzy.top/gtaxrlmwvb.html

[Q81] 字符串替换
来源：http://hz.jqgufenzy.top/gtjvcpmvhu.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.yj202588.top/gtmfpavmzz.html

[Q82] 字符长度与字节长度
来源：http://hz.sweek.top/gtmqkgwiwh.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.shanyushiyangkeji.top/gtvrrhjypt.html

[Q83] 大小写转换
来源：http://hz.guannengcc.top/gtqcrrszfi.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.zhoulong.xyz/gtkcyejmpz.html

[Q84] 去除首尾空格
来源：http://hz.nanxinkj.top/gtffojdhsu.html

SELECT TRIM(name) FROM users;
来源：http://hz.yangfankeji.com/gtrqyciwvb.html

[Q85] 数值取整
来源：http://hz.xuanzx.com/gtffokjejc.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.kuanghao11.cn/gtihqzcswn.html

[Q86] 读取 JSON 字段
来源：http://hz.dashuyun.cn/gtorwdzcit.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.hongshengwenyu.top/gtecncsmix.html

[Q87] JSON 字段做条件
来源：http://hz.9152youxi.cn/gtmwkcygtp.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.dianchejie.cn/gtnaggdikf.html

[Q88] 行转列（条件聚合）
来源：http://hz.meibo888.top/gtiethbyfv.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.yonumen.top/gttawpmrul.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.guannengcc.top/gtdvvexmea.html

[Q89] 判断表是否存在
来源：http://hz.sxryk.cn/gtzqmarbwo.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.zycfv.cn/gtjrmczmfj.html

[Q90] 生成序号列
来源：http://hz.jqgfzy.top/gtkqedezyr.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.zhaomingkeji.xyz/gtahjjtbdf.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtyhzlsucj.html

R. Bash 专题
来源：http://hz.ybcxt.top/gtsxedkylj.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtchofacms.html

[R01] shebang 与严格模式
来源：http://hz.hywenlv.cn/gtfzlcmfmh.html

#!/usr/bin/env bash
来源：http://hz.c1oappe.top/gtfqftgxih.html

set -euo pipefail
来源：http://hz.snrcjt.cn/gtmxdjqnlm.html

[R02] 变量赋值与使用
来源：http://hz.wangshuangyany.cn/gtcyijuwjw.html

name="Tom"; echo "$name"
来源：http://hz.yuanzhike.top/gtaeoomzpu.html

[R03] 只读变量
来源：http://hz.havefunace.top/gtwsuoisxk.html

readonly PI=3.14
来源：http://hz.shanyushiyangtech.top/gtzmkeyjaf.html

[R04] 位置参数
来源：http://hz.svipenyu.cn/gtspzibfna.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.pengpengdd.cyou/gtjeejofac.html

[R05] 参数默认值
来源：http://hz.cheryme.top/gthsripxab.html

name="${1:-default}"
来源：http://hz.zhaomingkeji.xyz/gttzeghwlu.html

[R06] 判断命令是否存在
来源：http://hz.smart0.xyz/gthgjskawb.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.wangshuangyany.cn/gtjucviezs.html

[R07] if 判断文件
来源：http://hz.shzxlz.cn/gtzojqpqhc.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.shanyushiyangtech.top/gtmcrrmidn.html

[R08] 数值比较
来源：http://hz.ywan-chungtsiang.top/gtsqpwoqia.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.aizwys.cn/gtcuwwbojz.html

[R09] 字符串比较
来源：http://hz.zhoulong.xyz/gtjlhnrpao.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.xuanzx.com/gtpoqdrrib.html

[R10] 正则匹配
来源：http://hz.xingfuxueyuan.xyz/gtqbsszrwz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.jqgfzy.top/gtcmsczxja.html

[R11] case 多分支
来源：http://hz.hammf.cn/gtrruhrayv.html

case "$1" in
来源：http://hz.kuanghao11.cn/gtkdhlsgno.html

start) echo "启动" ;;
来源：http://hz.shzxlz.cn/gtituvrhws.html

stop)  echo "停止" ;;
来源：http://hz.jiagoushi.top/gtuvrzgvrb.html

*)     echo "未知命令" ;;
来源：http://hz.zhoulong.xyz/gtcbtysufj.html

esac
来源：http://hz.gogol.net.cn/gtizegwntj.html

[R12] for 遍历文件
来源：http://hz.yj20258.top/gtyfzkcdfa.html

for f in *.txt; do echo "$f"; done
来源：http://hz.daria6918.cn/gtjxljrrvv.html

[R13] for 计数循环
来源：http://hz.xylfe.cn/gtkbijawsg.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.yangfankeji.com/gtehwlczvn.html

[R14] C 风格 for
来源：http://hz.hongshengwenyu.top/gtoqfhjgjo.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.andypj.xyz/gtqnangmbq.html

[R15] while 逐行读文件
来源：http://hz.jiagoushi.top/gtvfrrbrvc.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.ywan-chungtsiang.top/gtvcuqufxc.html

[R16] until 等待条件
来源：http://hz.quarkkingdee.top/gtavfgfgzz.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.jinyuanbaomall.cn/gtdhlmzsqt.html

[R17] 数组定义与取值
来源：http://hz.zdqjudy.top/gtedaunjni.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.jinqigufen.top/gtezdhleuc.html

[R18] 遍历数组
来源：http://hz.0kj1m.cn/gtlvwzrosr.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.yueranfly.top/gtfjzbpqkn.html

[R19] 数组长度
来源：http://hz.sufxvd.cn/gtyingsbnq.html

echo "${#arr[@]}"
来源：http://hz.quarkkingdee.top/gtxkgiiqzb.html

[R20] 关联数组（字典）
来源：http://hz.havefunace.top/gtanenxlnb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.yj20258888.top/gtzxhkihnd.html

[R21] 字符串长度
来源：http://hz.ivvv.top/gtwaiernrp.html

echo "${#s}"
来源：http://hz.xinyue.icu/gtbxjxxube.html

[R22] 截取子串
来源：http://hz.dashuyun.cn/gtikehnagx.html

echo "${s:0:5}"
来源：http://hz.aibaodan.cn/gtgqxebkwn.html

[R23] 字符串替换
来源：http://hz.zhoulong.xyz/gthpcognvm.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.xingfuxueyuan.xyz/gtoxeprdmk.html

[R24] 大小写转换
来源：http://hz.sxryk.cn/gtovecacgz.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.tianlin.xyz/gthevufkdy.html

[R25] 去后缀 / 去前缀
来源：http://hz.yj20258.top/gtxewjfglm.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.jiagoushi.top/gtnbjwzhbf.html

[R26] 命令替换
来源：http://hz.zdqjudy.top/gtsnvwdakz.html

now=$(date +%F); echo "$now"
来源：http://hz.zhixingplan.top/gtfofvmfal.html

[R27] 算术展开
来源：http://hz.havefunace.top/gtkmwobugm.html

echo $((1 + 2 * 3))
来源：http://hz.hnxiangtu.top/gtevrfkxmb.html

[R28] 浮点运算
来源：http://hz.tianlin.xyz/gthplxwaii.html

echo "scale=2; 10/3" | bc
来源：http://hz.yj202588.top/gtknjlytqa.html

[R29] 定义函数
来源：http://hz.tianlin.xyz/gtuxdfngvu.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.52xcode.cn/gtyqkgyntp.html

[R30] 函数返回状态码
来源：http://hz.guannengcc.top/gtterqufwg.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.yonumen.top/gtptskyact.html

[R31] 局部变量
来源：http://hz.zhengqikj.top/gtntpislcd.html

f() { local x=1; echo "$x"; }
来源：http://hz.xuanzx.com/gtccaoywif.html

[R32] 参数个数校验
来源：http://hz.gogol.net.cn/gttmztmpmp.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.fengsongda.top/gthxaguvfc.html

[R33] 捕获错误并提示行号
来源：http://hz.cdnleiting.top/gthqnmqnay.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.chenlongwang.top/gtwsvcrkly.html

[R34] 退出时清理
来源：http://hz.xuetiantiany.cn/gtvkthlneo.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.vqdsnc.cn/gtgcizjrpb.html

[R35] 后台执行并等待
来源：http://hz.gogol.net.cn/gtnyndeiqy.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.yueranfly.top/gtunyowgsf.html

[R36] 并发执行多个任务
来源：http://hz.smart0.xyz/gtqjflmmuh.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.daxiang520.top/gtaurxpuvu.html

[R37] 把输出赋给变量
来源：http://hz.daria6918.cn/gtkfkfmcwy.html

files=$(ls -1)
来源：http://hz.zhongyouzk.top/gtxpgxrpvg.html

[R38] 管道串联
来源：http://hz.fzhhl.top/gtyazmtdjd.html

cat a.txt | grep -i error | wc -l
来源：http://hz.sysykeji.top/gtpwaauoyo.html

[R39] 重定向标准输出与错误
来源：http://hz.sufxvd.cn/gthdioldby.html

cmd > out.log 2>&1
来源：http://hz.gogol.net.cn/gtwkxyswnu.html

[R40] 追加写日志
来源：http://hz.hywenlv.cn/gtjlgsumuq.html

echo "log" >> out.log
来源：http://hz.mhx1999.top/gtsaiuqsgf.html

[R41] 丢弃输出
来源：http://hz.nwbrower.top/gtdvhookws.html

cmd >/dev/null 2>&1
来源：http://hz.chenzaomai.com/gtnbwjjdzr.html

[R42] 输入重定向
来源：http://hz.xziqi.cn/gtbkrtgjxw.html

wc -l < a.txt
来源：http://hz.ybcxt.top/gtaihculfa.html

[R43] 按名字查找文件
来源：http://hz.gogol.net.cn/gtzaczvwmt.html

find . -name "*.log" -type f
来源：http://hz.zhixingplan.top/gtqpkkwwil.html

[R44] 按修改时间查找
来源：http://hz.yueranfly.top/gticbngtyx.html

find . -mtime -7 -type f
来源：http://hz.yvedp.cn/gtxwpofldr.html

[R45] 批量删除
来源：http://hz.sxryk.cn/gtritthlhg.html

find . -name "*.tmp" -delete
来源：http://hz.yueranfly.top/gtrfioejhl.html

[R46] 递归替换文件内容
来源：http://hz.gaohongyu789.top/gtxtazdrii.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.tian-w.cn/gtfmvrhrfc.html

[R47] sed 单行替换
来源：http://hz.jlsjyb.cn/gtwsfwvagz.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.meibo888.top/gtvqtisewr.html

[R48] awk 取指定列
来源：http://hz.shangyingyoupin.top/gtajtgjcxn.html

awk '{print $1, $3}' a.txt
来源：http://hz.shanyushiyangtech.top/gtkuzeblke.html

[R49] awk 带条件
来源：http://hz.fengsongda.top/gtkvqnwbej.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.jiagoushi.top/gtttbdlkar.html

[R50] awk 求和
来源：http://hz.cucudq.cn/gtnwafsmod.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.zdqjudy.top/gtpiajxfux.html

[R51] 排序去重取前几
来源：http://hz.52xcode.cn/gthrlzpnky.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.zdqjudy.top/gtmzvnlhub.html

[R52] 统计行数
来源：http://hz.hfpthk.cn/gtxvksycyh.html

wc -l a.txt
来源：http://hz.hywenlv.cn/gttvhitshk.html

[R53] 查看文件头与实时尾
来源：http://hz.tian-w.cn/gtddjgtyon.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.yvedp.cn/gtqvqjtlbk.html

[R54] 比较两个文件
来源：http://hz.cqqwz.cn/gtbkolkpqe.html

diff a.txt b.txt
来源：http://hz.cqqwz.cn/gtqptugega.html

[R55] 压缩与解压
来源：http://hz.ybcxt.top/gtxpdnidxg.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.yj20258.top/gteuwdxeyv.html

[R56] 远程拷贝
来源：http://hz.shanyushiyangkeji.top/gtcpoyymuc.html

scp file user@host:/path/
来源：http://hz.shanyushiyangkeji.top/gtcxecqtjl.html

[R57] 远程执行命令
来源：http://hz.pengpengdd.cyou/gtatrhjqqc.html

ssh user@host 'uptime'
来源：http://hz.svipenyu.cn/gteddptmlc.html

[R58] 下载文件
来源：http://hz.feifeiyinyue.top/gtefsycdes.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.quarkkingdee.top/gtixolupdr.html

[R59] 发 POST JSON
来源：http://hz.shuidangran.top/gtibpqffrv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.sysykeji.top/gtaoevbodq.html

[R60] 只看 HTTP 状态码
来源：http://hz.cdnleiting.top/gtdjzpnsvb.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.zycfv.cn/gtzggpmggt.html

[R61] 磁盘占用
来源：http://hz.sxryk.cn/gtpfqnpinh.html

df -h;  du -sh *
来源：http://hz.hywenlv.cn/gtghqwarqn.html

[R62] 找最占空间的文件
来源：http://hz.yongpay.top/gtvnkqdlpd.html

du -ah . | sort -rh | head -10
来源：http://hz.zhengqikj.top/gtjckvowfs.html

[R63] 内存与进程
来源：http://hz.shangyingyoupin.top/gtyfpcuhtf.html

free -h;  ps aux | grep nginx
来源：http://hz.fengsongda.top/gtudfdzjcj.html

[R64] 结束进程
来源：http://hz.jinqigfzy.top/gthedjgxfo.html

kill -9 $(pgrep -f app.py)
来源：http://hz.daria6918.cn/gtrdogrija.html

[R65] 查看端口占用
来源：http://hz.chenlongwang.top/gtzhafphto.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.cucudq.cn/gtljamifcm.html

[R66] 定时任务
来源：http://hz.jqgfzy.top/gtvahfcufo.html

crontab -e;  crontab -l
来源：http://hz.zhaomingkeji.xyz/gttryhaalk.html

[R67] 生成随机十六进制串
来源：http://hz.ehwqpu.com/gtlnfwnjms.html

openssl rand -hex 16
来源：http://hz.shangyingyoupin.top/gthxbcrlsw.html

[R68] 计算文件校验值
来源：http://hz.nanxinkj.top/gtpalgymgw.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.sxryk.cn/gtnohzphrb.html

[R69] 生成随机密码
来源：http://hz.wangshuangyany.cn/gtgatgcvch.html

head -c 16 /dev/urandom | base64
来源：http://hz.yj202588.top/gtudbixoqa.html

[R70] 时间戳与互转
来源：http://hz.nanxuanxn.top/gtngeenkky.html

date +%s;  date -d @1700000000
来源：http://hz.xuetiantiany.cn/gttuzhoxvt.html

[R71] 日期格式化
来源：http://hz.kuanghao11.cn/gtbuokynvi.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.cqqwz.cn/gtpcxxxyua.html

[R72] 等待端口就绪
来源：http://hz.yj202588.top/gtqkqvxuew.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.yueranfly.top/gtznwwiioi.html

[R73] 分割大日志
来源：http://hz.0kj1m.cn/gtxuewjgow.html

split -l 1000 big.log part_
来源：http://hz.jinghuilouyu.cn/gtlnrgchsz.html

[R74] 批量重命名
来源：http://hz.quarkkingdee.top/gtkzdexrau.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.yj20258888.top/gtcoreeozd.html

[R75] 导出环境变量
来源：http://hz.cdnleiting.top/gtidjsthuh.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.hongshengwenyu.top/gtdyncbodq.html

[R76] 使用临时文件
来源：http://hz.yj20258.top/gtpzsgnaxv.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.jinqigfzy.top/gtjyxovqiv.html

[R77] 读取用户输入
来源：http://hz.andypj.xyz/gtqhksnguc.html

read -rp "请输入: " ans
来源：http://hz.fzhhl.top/gtzeacnfai.html

[R78] 交互式菜单
来源：http://hz.chenlongwang.top/gthpyxtczq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.kuanghao11.cn/gtaxibzmab.html

[R79] 解析命令行选项
来源：http://hz.yuanzhike.top/gtnlkehacy.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.tanke756.top/gtiklutnwr.html

[R80] 查看脚本执行耗时
来源：http://hz.zhiwuduotai.top/gtxzljskop.html

time ./run.sh
来源：http://hz.ywan-chungtsiang.top/gtgeiloqcw.html

================================================================================
来源：http://hz.gzhubu.top/gtsaivkozl.html

S. C / C++ 专题
来源：http://hz.hysaishi.cn/gtuoigbzun.html

================================================================================
来源：http://hz.cdnleiting.top/gtecjiyvpo.html

[S01] C：Hello World
来源：http://hz.hfpthk.cn/gtbtbrgkvo.html

#include <stdio.h>
来源：http://hz.yj20258.top/gtrnlkbrbm.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.redwolf501.top/gtfcicevqw.html

[S02] C：变量与格式化输出
来源：http://hz.smart0.xyz/gtbofyrsgv.html

int a = 10; printf("%d\n", a);
来源：http://hz.zhiwuduotai.top/gtvpmxgjqe.html

[S03] C：读入整数
来源：http://hz.zhixingplan.top/gtwrwkhgqp.html

int x; scanf("%d", &x);
来源：http://hz.xingfuxueyuan.xyz/gtoplpepxk.html

[S04] C：字符串复制
来源：http://hz.ivvv.top/gtpefyeehe.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.aibaodan.cn/gtsvliirkv.html

[S05] C：字符串长度
来源：http://hz.meibo888.top/gtndibmncc.html

strlen(s)
来源：http://hz.xingfuxueyuan.xyz/gtbahpibix.html

[S06] C：字符串比较
来源：http://hz.ppjwa.cn/gtwznnsjed.html

strcmp(a, b) == 0
来源：http://hz.c1oappe.top/gtntmehxfm.html

[S07] C：数组遍历求和
来源：http://hz.0kj1m.cn/gtvtoljdoh.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.ybcxt.top/gtjwrdnlgc.html

[S08] C：动态内存分配与释放
来源：http://hz.zhixingplan.top/gtyuwiqeua.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.gaohongyu789.top/gtoyrsyedm.html

[S09] C：结构体定义与初始化
来源：http://hz.shanyushiyangkeji.top/gtyocrbmiz.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.jqgfzy.top/gtktibweve.html

[S10] C：指针与解引用
来源：http://hz.zdqjudy.top/gttwrnpgjv.html

int *p = &a;  *p = 5;
来源：http://hz.aibaodan.cn/gttpgsaryp.html

[S11] C：逐行读文件
来源：http://hz.zhaomingkeji.xyz/gtuyiswnvb.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.ywan-chungtsiang.top/gtsmgvtado.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.jqgfzy.top/gthxblewsd.html

fclose(f);
来源：http://hz.wangshuangyany.cn/gtfafhyutd.html

[S12] C：写文件
来源：http://hz.bjfxy.top/gtpwtjfdgm.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.yj20258888.top/gtybexofxc.html

[S13] C：宏定义
来源：http://hz.snrcjt.cn/gtkpceqxml.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.zdqjudy.top/gttsostesf.html

[S14] C：枚举
来源：http://hz.ydzc1.top/gtzxrbseiu.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.zycfv.cn/gtdjlmnvmp.html

[S15] C：类型转换
来源：http://hz.nanxuanxn.top/gtivbukqfe.html

(double) a / b
来源：http://hz.ydjk.org.cn/gtdwdgwrrw.html

[S16] C：位操作置位
来源：http://hz.zdqjudy.top/gtqnbxeoct.html

x |= (1 << 3);
来源：http://hz.hnxiangtu.top/gtsqzcvtku.html

[S17] C：安全拼接字符串
来源：http://hz.ydzc1.top/gtcjgzrxhl.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.nanxinkj.top/gtsrvjmnep.html

[S18] C：命令行参数
来源：http://hz.cucudq.cn/gtdxatcujk.html

int main(int argc, char **argv)
来源：http://hz.smart0.xyz/gtwpqrbmhf.html

[S19] C：快速排序
来源：http://hz.dashuyun.cn/gtuxoykszp.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.0kj1m.cn/gtipispdsr.html

[S20] C：二分查找
来源：http://hz.yanxiufei.cn/gtptubtipr.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.zhaomingkeji.xyz/gtssundqjb.html

[S21] C：字符类别判断
来源：http://hz.xziqi.cn/gtnelkrfcg.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.shangyingyoupin.top/gtnfdrxqma.html

[S22] C：字符串转数字
来源：http://hz.svipenyu.cn/gttxibvugd.html


<!-- 参考信息 -->