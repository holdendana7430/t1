代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.chenzaomai.com/gtufgvktdn.html

[Q50] 批量更新
来源：http://hz.hnqzz.top/gtpqkrsnps.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.chenzaomai.com/gtipjdcbts.html

[Q51] 用子查询更新
来源：http://hz.xinyue.icu/gtiqeogleq.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.pengpengdd.cyou/gtlqofdjtu.html

[Q52] 删除指定行
来源：http://hz.zhengqikj.top/gtpgxguekn.html

DELETE FROM users WHERE id = 10;
来源：http://hz.jinqigfzy.top/gttzdkrisa.html

[Q53] 按条件删除
来源：http://hz.cdnleiting.top/gtdqbfewhz.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.jianghu66.top/gtfldkczcf.html

[Q54] 清空表
来源：http://hz.ydjk.org.cn/gtxgrqqepa.html

TRUNCATE TABLE logs;
来源：http://hz.hysaishi.cn/gtjdfzuyse.html

[Q55] 排名（并列占位）
来源：http://hz.andypj.xyz/gtfwewfqtf.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.svipenyu.cn/gtentxwydu.html

[Q56] 密集排名（并列不占位）
来源：http://hz.hfpthk.cn/gtkjjkjpko.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.yj202588.top/gtxxguefbw.html

[Q57] 行号
来源：http://hz.yuxming.cn/gtdtlxsicu.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.cucudq.cn/gtjtxqlnfi.html

[Q58] 累计求和
来源：http://hz.chenjidiqi.icu/gtqvtnphqe.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.ivvv.top/gtogcsixop.html

[Q59] 分组内累计
来源：http://hz.ywan-chungtsiang.top/gtnjnboxji.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.mhx1999.top/gtjtdkmkul.html

[Q60] 取上一行 / 下一行
来源：http://hz.yanxiufei.cn/gtnrrthcyx.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.shanyushiyangtech.top/gtanbmwann.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.ydzc1.top/gtqlzskbdw.html

[Q61] 移动平均
来源：http://hz.ivvv.top/gtmnnhyred.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.hfpthk.cn/gtjswneazg.html

[Q62] 分组占比
来源：http://hz.52xcode.cn/gtvaxbnzpd.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.sufxvd.cn/gtamfiyids.html

[Q63] 开启事务
来源：http://hz.xziqi.cn/gtehoiivcm.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.kuanghao11.cn/gtfaxkzorb.html

[Q64] 提交事务
来源：http://hz.jqgfzy.top/gtkberzkcn.html

COMMIT;
来源：http://hz.haohaochexian.top/gtvzqpjxrd.html

[Q65] 回滚事务
来源：http://hz.yuxming.cn/gtipusrlsn.html

ROLLBACK;
来源：http://hz.fengsongda.top/gtgekoeont.html

[Q66] 行锁查询
来源：http://hz.ivvv.top/gtomgcexdb.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.wangshuangyany.cn/gtoeiifwep.html

[Q67] 设置隔离级别
来源：http://hz.cucudq.cn/gtwycogawj.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.redwolf501.top/gtuevttuke.html

[Q68] 保存点
来源：http://hz.jlsjyb.cn/gtvegvtmqe.html

SAVEPOINT sp1;
来源：http://hz.jiagoushi.top/gtyjcwcfeg.html

ROLLBACK TO sp1;
来源：http://hz.yj20258.top/gtwesthcqu.html

[Q69] 查看执行计划
来源：http://hz.zhaomingkeji.xyz/gtdziihjib.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.hfpthk.cn/gtkwevrgrs.html

[Q70] 更新统计信息
来源：http://hz.nanxinkj.top/gtvphrroyt.html

ANALYZE TABLE users;
来源：http://hz.cqqwz.cn/gtanyaofvn.html

[Q71] 查看建表语句
来源：http://hz.gogol.net.cn/gtcfixdrya.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.c1oappe.top/gtwwmyahch.html

[Q72] 查看索引
来源：http://hz.ydzc1.top/gtwtckezml.html

SHOW INDEX FROM users;
来源：http://hz.wangdashe.top/gtzbnldjpv.html

[Q73] 查看表状态
来源：http://hz.hongshengwenyu.top/gtedkdjtaa.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.cdnleiting.top/gtvsgkqrdh.html

[Q74] 强制使用索引
来源：http://hz.haohaochexian.top/gtvmepfjnq.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.guowangkeji.top/gtxlynuexc.html

[Q75] 日期格式化
来源：http://hz.cqqwz.cn/gtjfnzcvxx.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.nwbrower.top/gtkfcmuzej.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.snrcjt.cn/gthvrkzqdu.html

[Q76] 按天统计
来源：http://hz.gotoacloud.top/gtyacsiliq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.tianlin.xyz/gtmnmcdnbt.html

[Q77] 时间加减
来源：http://hz.sxryk.cn/gteayocqph.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.vqdsnc.cn/gtneuvaqbw.html

[Q78] 当前时间
来源：http://hz.meibo888.top/gtebxqcdjn.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.cucudq.cn/gtxskrfiak.html

[Q79] 字符串拼接
来源：http://hz.zhijiandao.cn/gtqqcfaiuc.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.nanxinkj.top/gtmwpdkztc.html

[Q80] 字符串截取
来源：http://hz.nanxuanxn.top/gtdqdbqarc.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.sxryk.cn/gtdyvlbcui.html

[Q81] 字符串替换
来源：http://hz.ehwqpu.com/gtxdkyeyco.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.sufxvd.cn/gtjltotoxu.html

[Q82] 字符长度与字节长度
来源：http://hz.yuanzhike.top/gtnhhvlmve.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.yvedp.cn/gtlajfpauo.html

[Q83] 大小写转换
来源：http://hz.yongpay.top/gtvrewadkm.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.iojbl.cn/gtyulsvsid.html

[Q84] 去除首尾空格
来源：http://hz.bjfxy.top/gttarivwmd.html

SELECT TRIM(name) FROM users;
来源：http://hz.zdqjudy.top/gtindqcteu.html

[Q85] 数值取整
来源：http://hz.yj20258888.top/gtssdvmiye.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.yangfankeji.com/gtohgixmkh.html

[Q86] 读取 JSON 字段
来源：http://hz.chenlongwang.top/gtphiybkxz.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.ywan-chungtsiang.top/gtatucloyr.html

[Q87] JSON 字段做条件
来源：http://hz.dashuyun.cn/gtdrkaliie.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.jinqigfzy.top/gthhxaolib.html

[Q88] 行转列（条件聚合）
来源：http://hz.hammf.cn/gtxjryayzv.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.svipenyu.cn/gtpnyrescp.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.shanyushiyangkeji.top/gtcwrdcgze.html

[Q89] 判断表是否存在
来源：http://hz.zhijiandao.cn/gtuhffnsya.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.hfpthk.cn/gtwgbnvlnt.html

[Q90] 生成序号列
来源：http://hz.shanyushiyangtech.top/gtzbsvdqhb.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.cucudq.cn/gtwhavbpqc.html

================================================================================
来源：http://hz.svipenyu.cn/gtrpogucfd.html

R. Bash 专题
来源：http://hz.ivvv.top/gtmnwivkje.html

================================================================================
来源：http://hz.sweek.top/gtlvtkoftc.html

[R01] shebang 与严格模式
来源：http://hz.jianghu66.top/gtnjcknarq.html

#!/usr/bin/env bash
来源：http://hz.hammf.cn/gtadqdjglg.html

set -euo pipefail
来源：http://hz.xylfe.cn/gtdffatbwe.html

[R02] 变量赋值与使用
来源：http://hz.zhongyouzk.top/gthdxliabm.html

name="Tom"; echo "$name"
来源：http://hz.gotoacloud.top/gtcuqbtfna.html

[R03] 只读变量
来源：http://hz.sufxvd.cn/gtpwermdiq.html

readonly PI=3.14
来源：http://hz.redwolf501.top/gtblsntucs.html

[R04] 位置参数
来源：http://hz.ppjwa.cn/gtivlaqhhl.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.nwbrower.top/gttpumjdam.html

[R05] 参数默认值
来源：http://hz.sweek.top/gtionbeqez.html

name="${1:-default}"
来源：http://hz.mhx1999.top/gteofcbsyi.html

[R06] 判断命令是否存在
来源：http://hz.chenlongwang.top/gtdzeqlrqs.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.yanxiufei.cn/gtldidlpqi.html

[R07] if 判断文件
来源：http://hz.xinyue.icu/gtumqtlbdj.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.yanxiufei.cn/gtcqfxxlne.html

[R08] 数值比较
来源：http://hz.ppjwa.cn/gtezttcxmi.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.jinqigufen.top/gtybdgkazg.html

[R09] 字符串比较
来源：http://hz.feifeiyinyue.top/gtdqozrhke.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.9152youxi.cn/gtnukycrli.html

[R10] 正则匹配
来源：http://hz.sweek.top/gtazuoozxv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.zdqjudy.top/gtaurzblne.html

[R11] case 多分支
来源：http://hz.hnqzz.top/gtwwmshtwl.html

case "$1" in
来源：http://hz.wangshuangyany.cn/gtcndiyxpd.html

start) echo "启动" ;;
来源：http://hz.ppjwa.cn/gtvuuzfhnv.html

stop)  echo "停止" ;;
来源：http://hz.xinyue.icu/gtfbriamix.html

*)     echo "未知命令" ;;
来源：http://hz.cheryme.top/gtdonpkyud.html

esac
来源：http://hz.jinghuilouyu.cn/gtjeuecujb.html

[R12] for 遍历文件
来源：http://hz.tanke756.top/gtzfqxujcw.html

for f in *.txt; do echo "$f"; done
来源：http://hz.jinyuanbaomall.cn/gtjbduckqn.html

[R13] for 计数循环
来源：http://hz.yueranfly.top/gtinilqczc.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.shanyushiyangtech.top/gtzrdifuek.html

[R14] C 风格 for
来源：http://hz.xuetiantiany.cn/gtlsrivlvc.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.yj202588.top/gtkflypxhb.html

[R15] while 逐行读文件
来源：http://hz.smart0.xyz/gtqxtkjxkc.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.yvedp.cn/gtttobixnb.html

[R16] until 等待条件
来源：http://hz.nwbrower.top/gtnzkhheqq.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.chenzaomai.com/gtfthuggfz.html

[R17] 数组定义与取值
来源：http://hz.nwbrower.top/gtkqqqyytf.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.gotoacloud.top/gtbupbaxcb.html

[R18] 遍历数组
来源：http://hz.smart0.xyz/gtxlileays.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.316326.xyz/gthwshewjg.html

[R19] 数组长度
来源：http://hz.ydzc1.top/gtjsfaspse.html

echo "${#arr[@]}"
来源：http://hz.guannengcc.top/gteuerkbzi.html

[R20] 关联数组（字典）
来源：http://hz.yangfankeji.com/gtrkqbvlqo.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.sweek.top/gtqjidavxd.html

[R21] 字符串长度
来源：http://hz.jinqigfzy.top/gtjinwlqll.html

echo "${#s}"
来源：http://hz.haohaochexian.top/gtubpggtsl.html

[R22] 截取子串
来源：http://hz.jinyuanbaomall.cn/gtgqdojgkf.html

echo "${s:0:5}"
来源：http://hz.jinyuanbaomall.cn/gtrpfaiirr.html

[R23] 字符串替换
来源：http://hz.hysaishi.cn/gtcsusdbun.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.sxryk.cn/gtlabwwwad.html

[R24] 大小写转换
来源：http://hz.ywan-chungtsiang.top/gtkmsicejr.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.xingfuxueyuan.xyz/gtzjnudvei.html

[R25] 去后缀 / 去前缀
来源：http://hz.yonumen.top/gtyqwwsyqt.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.chenzaomai.com/gtjzyfsrcu.html

[R26] 命令替换
来源：http://hz.gogol.net.cn/gtanqydwnz.html

now=$(date +%F); echo "$now"
来源：http://hz.wangshuangyany.cn/gtznhucexk.html

[R27] 算术展开
来源：http://hz.sysykeji.top/gtsthdbyfr.html

echo $((1 + 2 * 3))
来源：http://hz.yj20258888.top/gtgvajsfqh.html

[R28] 浮点运算
来源：http://hz.jlsjyb.cn/gtbcdoqzje.html

echo "scale=2; 10/3" | bc
来源：http://hz.chenzaomai.com/gtsmkeebzv.html

[R29] 定义函数
来源：http://hz.nanxinkj.top/gteajbimsf.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.xuetiantiany.cn/gtselcrnaz.html

[R30] 函数返回状态码
来源：http://hz.daria6918.cn/gtgyhpfxup.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.hfpthk.cn/gtajofxssi.html

[R31] 局部变量
来源：http://hz.sufxvd.cn/gtetwuueyr.html

f() { local x=1; echo "$x"; }
来源：http://hz.yuxming.cn/gtfeuocmpk.html

[R32] 参数个数校验
来源：http://hz.52xcode.cn/gturaiypro.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.feifeiyinyue.top/gtgqdatlyz.html

[R33] 捕获错误并提示行号
来源：http://hz.jqgufenzy.top/gtfmuivgkg.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.zycfv.cn/gthdzgqmyj.html

[R34] 退出时清理
来源：http://hz.chenzaomai.com/gtnzdajxqk.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.cucudq.cn/gtdmreqidg.html

[R35] 后台执行并等待
来源：http://hz.cucudq.cn/gtamtmytgc.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.dianchejie.cn/gtygguqhnl.html

[R36] 并发执行多个任务
来源：http://hz.hammf.cn/gtbmmddqgj.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.hysaishi.cn/gtrcqsajrv.html

[R37] 把输出赋给变量
来源：http://hz.smart0.xyz/gtiavqkfqw.html

files=$(ls -1)
来源：http://hz.pycfn.com/gtnmditqns.html

[R38] 管道串联
来源：http://hz.yonumen.top/gthypabsjq.html

cat a.txt | grep -i error | wc -l
来源：http://hz.ehwqpu.com/gtwfblssal.html

[R39] 重定向标准输出与错误
来源：http://hz.yueranfly.top/gtpflzxxpt.html

cmd > out.log 2>&1
来源：http://hz.xylfe.cn/gtvilmpqdp.html

[R40] 追加写日志
来源：http://hz.birdmap.top/gtwcoogsac.html

echo "log" >> out.log
来源：http://hz.nwbrower.top/gtvmagimuh.html

[R41] 丢弃输出
来源：http://hz.hfpthk.cn/gtndsstmyn.html

cmd >/dev/null 2>&1
来源：http://hz.ydjk.org.cn/gthotclklz.html

[R42] 输入重定向
来源：http://hz.yj20258.top/gtbsjkmkar.html

wc -l < a.txt
来源：http://hz.nanxinkj.top/gtrwxpxmwd.html

[R43] 按名字查找文件
来源：http://hz.svipenyu.cn/gtkdvlwfoy.html

find . -name "*.log" -type f
来源：http://hz.fengsongda.top/gtjmndbkap.html

[R44] 按修改时间查找
来源：http://hz.vqdsnc.cn/gtekybxsrv.html

find . -mtime -7 -type f
来源：http://hz.jiagoushi.top/gtymucapex.html

[R45] 批量删除
来源：http://hz.cashguo.top/gtxvitmrtf.html

find . -name "*.tmp" -delete
来源：http://hz.shanyushiyangtech.top/gtszvnostu.html

[R46] 递归替换文件内容
来源：http://hz.jinyuanbaomall.cn/gtvzjcvcqc.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.tian-w.cn/gttwzuvroq.html

[R47] sed 单行替换
来源：http://hz.daria6918.cn/gtutacjlfn.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.yanxiufei.cn/gtzvvuiimd.html

[R48] awk 取指定列
来源：http://hz.xziqi.cn/gtsgnsucly.html

awk '{print $1, $3}' a.txt
来源：http://hz.0kj1m.cn/gtjrnstaji.html

[R49] awk 带条件
来源：http://hz.52xcode.cn/gtzfidtosj.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.haohaochexian.top/gtkvxejheh.html

[R50] awk 求和
来源：http://hz.hnxiangtu.top/gtqtzsuxze.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.shanyushiyangtech.top/gtyecdrlxu.html

[R51] 排序去重取前几
来源：http://hz.yj20258888.top/gtclautmkq.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.hnxiangtu.top/gtypmsmbhv.html

[R52] 统计行数
来源：http://hz.nanxuanxn.top/gtqsmyjiix.html

wc -l a.txt
来源：http://hz.yonumen.top/gtgbknyatr.html

[R53] 查看文件头与实时尾
来源：http://hz.fzhhl.top/gttepdeeku.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.yuanzhike.top/gtbrycoxyb.html

[R54] 比较两个文件
来源：http://hz.svipenyu.cn/gtbtszclfp.html

diff a.txt b.txt
来源：http://hz.cqqwz.cn/gtjhccyvel.html

[R55] 压缩与解压
来源：http://hz.zhaomingkeji.xyz/gtvjtbrhhi.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.hnxiangtu.top/gtqzzkumrj.html

[R56] 远程拷贝
来源：http://hz.xinyue.icu/gtgjkljjgm.html

scp file user@host:/path/
来源：http://hz.havefunace.top/gtrnpjbbuj.html

[R57] 远程执行命令
来源：http://hz.zdqjudy.top/gtjsanhfml.html

ssh user@host 'uptime'
来源：http://hz.0kj1m.cn/gtscxupvfw.html

[R58] 下载文件
来源：http://hz.yonumen.top/gtdceigvke.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.gotoacloud.top/gtiobzagnb.html

[R59] 发 POST JSON
来源：http://hz.smart0.xyz/gtkzgkxiso.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.fzhhl.top/gtyryosepc.html

[R60] 只看 HTTP 状态码
来源：http://hz.svipenyu.cn/gtlmhbtoll.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.birdmap.top/gtqkzjsxna.html

[R61] 磁盘占用
来源：http://hz.bjfxy.top/gtazqsxalg.html

df -h;  du -sh *
来源：http://hz.hysaishi.cn/gtgsytpahv.html

[R62] 找最占空间的文件
来源：http://hz.jinqigufen.top/gtzagoxxxu.html

du -ah . | sort -rh | head -10
来源：http://hz.sxryk.cn/gtjbafrgzu.html

[R63] 内存与进程
来源：http://hz.snrcjt.cn/gtikkbhawh.html

free -h;  ps aux | grep nginx
来源：http://hz.ehwqpu.com/gtvwwbtvoc.html

[R64] 结束进程
来源：http://hz.gzhubu.top/gtpzfrnxzr.html

kill -9 $(pgrep -f app.py)
来源：http://hz.gaohongyu789.top/gtlrumkfjj.html

[R65] 查看端口占用
来源：http://hz.hnqzz.top/gtlokmrvqe.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.shanyushiyangkeji.top/gtepmwrjkw.html

[R66] 定时任务
来源：http://hz.gzhubu.top/gtfljrazpq.html

crontab -e;  crontab -l
来源：http://hz.haohaochexian.top/gtvkqfdgqp.html

[R67] 生成随机十六进制串
来源：http://hz.haohaochexian.top/gtbjtpxofr.html

openssl rand -hex 16
来源：http://hz.quarkkingdee.top/gtxekqnezz.html

[R68] 计算文件校验值
来源：http://hz.zhongyouzk.top/gtuvlhudgb.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.snrcjt.cn/gtiueccfmr.html

[R69] 生成随机密码
来源：http://hz.shangyingyoupin.top/gtkxaiqraa.html

head -c 16 /dev/urandom | base64
来源：http://hz.shzxlz.cn/gthcufzdto.html

[R70] 时间戳与互转
来源：http://hz.yj202588.top/gtxbwkjqpp.html

date +%s;  date -d @1700000000
来源：http://hz.quarkkingdee.top/gtmdbgtbzf.html

[R71] 日期格式化
来源：http://hz.wangdashe.top/gtlttltbum.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.sysykeji.top/gteilzqtwg.html

[R72] 等待端口就绪
来源：http://hz.xziqi.cn/gtbuleknby.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.jinghuilouyu.cn/gtnuqpamfn.html

[R73] 分割大日志
来源：http://hz.zhiwuduotai.top/gtwmnjyvtv.html

split -l 1000 big.log part_
来源：http://hz.tianlin.xyz/gtqqawofpe.html

[R74] 批量重命名
来源：http://hz.xylfe.cn/gtexycwicz.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.dashuyun.cn/gtfcvftzvy.html

[R75] 导出环境变量
来源：http://hz.shanyushiyangtech.top/gtykdbomcl.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.birdmap.top/gtdlwalpoa.html

[R76] 使用临时文件
来源：http://hz.zhongyouzk.top/gtjahwnyga.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.bjfxy.top/gtuyqvsakh.html

[R77] 读取用户输入
来源：http://hz.jinqigfzy.top/gtiwicubax.html

read -rp "请输入: " ans
来源：http://hz.havefunace.top/gtdchxpwsx.html

[R78] 交互式菜单
来源：http://hz.jinqigufen.top/gthftowdac.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.yangfankeji.com/gtcijdcfcz.html

[R79] 解析命令行选项
来源：http://hz.ehwqpu.com/gtcedqegyc.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.hnxiangtu.top/gtqestlmnx.html

[R80] 查看脚本执行耗时
来源：http://hz.ivvv.top/gtgvlkqvpu.html

time ./run.sh
来源：http://hz.xziqi.cn/gtegwqaehe.html

================================================================================
来源：http://hz.cqqwz.cn/gtqzpjlqea.html

S. C / C++ 专题
来源：http://hz.svipenyu.cn/gthldhvwxz.html

================================================================================
来源：http://hz.52xcode.cn/gtvndiyrhx.html

[S01] C：Hello World
来源：http://hz.vqdsnc.cn/gtwjkcsfek.html

#include <stdio.h>
来源：http://hz.redwolf501.top/gtjlvnqnjl.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.cdnleiting.top/gtpzjujitt.html

[S02] C：变量与格式化输出
来源：http://hz.sysykeji.top/gtyohheckk.html

int a = 10; printf("%d\n", a);
来源：http://hz.kuanghao11.cn/gttckgugec.html

[S03] C：读入整数
来源：http://hz.aizwys.cn/gtsnnfliwg.html

int x; scanf("%d", &x);
来源：http://hz.tian-w.cn/gtvuzswfzd.html

[S04] C：字符串复制
来源：http://hz.tian-w.cn/gtwfqqgapw.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.zdqjudy.top/gtdjrypayj.html

[S05] C：字符串长度
来源：http://hz.tianlin.xyz/gtaosmfzhb.html

strlen(s)
来源：http://hz.ppjwa.cn/gtamzjoiar.html

[S06] C：字符串比较
来源：http://hz.jinqigfzy.top/gtuqglzzmj.html

strcmp(a, b) == 0
来源：http://hz.xuetiantiany.cn/gtmcwjmrvy.html

[S07] C：数组遍历求和
来源：http://hz.jinqigufen.top/gtwdkfwcbh.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.52xcode.cn/gtqejjolwp.html

[S08] C：动态内存分配与释放
来源：http://hz.guowangkeji.top/gtjmuqkvwb.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.xziqi.cn/gtzwgeaaer.html

[S09] C：结构体定义与初始化
来源：http://hz.jqgfzy.top/gtnhebnhpe.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.havefunace.top/gtwregulhv.html

[S10] C：指针与解引用
来源：http://hz.zhijiandao.cn/gtfqrzbolr.html

int *p = &a;  *p = 5;
来源：http://hz.zdqjudy.top/gtnjzvpkam.html

[S11] C：逐行读文件
来源：http://hz.316326.xyz/gtwlqmitzz.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.havefunace.top/gtnystncqy.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.zhiwuduotai.top/gtqronnkqj.html

fclose(f);
来源：http://hz.chenzaomai.com/gtmuyaxdsd.html

[S12] C：写文件
来源：http://hz.hfpthk.cn/gtgehphnae.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.chenzaomai.com/gtvdbigqho.html

[S13] C：宏定义
来源：http://hz.jqgufenzy.top/gtwcwtotxv.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.xuanzx.com/gtditjyatx.html

[S14] C：枚举
来源：http://hz.0kj1m.cn/gtuufrgfth.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.gaohongyu789.top/gtfvqxnksn.html

[S15] C：类型转换
来源：http://hz.chenjidiqi.icu/gtotudjvad.html

(double) a / b
来源：http://hz.cdnleiting.top/gtsuiyaoaf.html

[S16] C：位操作置位
来源：http://hz.hammf.cn/gtuiomwnmw.html

x |= (1 << 3);
来源：http://hz.fzhhl.top/gtkmbzsmra.html

[S17] C：安全拼接字符串
来源：http://hz.svipenyu.cn/gtmqhmeeiy.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.xinyue.icu/gtsnsjpmzl.html

[S18] C：命令行参数
来源：http://hz.xinyue.icu/gtgcguaoep.html

int main(int argc, char **argv)
来源：http://hz.sxryk.cn/gttvzjqudb.html

[S19] C：快速排序
来源：http://hz.dianchejie.cn/gtdnmsibcl.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.daria6918.cn/gtjmquhoqd.html

[S20] C：二分查找
来源：http://hz.fengsongda.top/gtcqofljzj.html


<!-- 参考信息 -->