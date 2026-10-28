代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://hz.pengpengdd.cyou/gtxhzhuhnh.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.nanxinkj.top/gtowtfcvof.html

[Q47] 与平均值比较
来源：http://hz.gotoacloud.top/gtrlvzcace.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.c1oappe.top/gtsblvnlzy.html

[Q48] CTE 公用表表达式
来源：http://hz.shangyingyoupin.top/gthyauluod.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.yj202588.top/gtrjcdyqgi.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.andypj.xyz/gtbjdueqhi.html

[Q49] 更新单行
来源：http://hz.316326.xyz/gtgyaifidr.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.yj202588.top/gteflcnikx.html

[Q50] 批量更新
来源：http://hz.yanxiufei.cn/gtjmndytek.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.aizwys.cn/gtgxybayoy.html

[Q51] 用子查询更新
来源：http://hz.sysykeji.top/gtgynglvbk.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.iojbl.cn/gtcobldvkk.html

[Q52] 删除指定行
来源：http://hz.zhaomingkeji.xyz/gtubwcjuxb.html

DELETE FROM users WHERE id = 10;
来源：http://hz.zhengqikj.top/gtxqmjpscf.html

[Q53] 按条件删除
来源：http://hz.jyoumei.cn/gtqibiouei.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.ydzc1.top/gtbzpchoju.html

[Q54] 清空表
来源：http://hz.jqgfzy.top/gthivijpkc.html

TRUNCATE TABLE logs;
来源：http://hz.chenjidiqi.icu/gtlltcfhuv.html

[Q55] 排名（并列占位）
来源：http://hz.iojbl.cn/gtrucxlazz.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.cheryme.top/gtutsvaqwb.html

[Q56] 密集排名（并列不占位）
来源：http://hz.0kj1m.cn/gtbygshlmm.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.yuxming.cn/gtffmmbvrq.html

[Q57] 行号
来源：http://hz.jinqigufen.top/gtcdrutrsi.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.guannengcc.top/gtxhdhmeky.html

[Q58] 累计求和
来源：http://hz.chenzaomai.com/gthsqipfef.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.birdmap.top/gtnoydhtrd.html

[Q59] 分组内累计
来源：http://hz.yvedp.cn/gtmwnhokbo.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.sweek.top/gtqbarpacr.html

[Q60] 取上一行 / 下一行
来源：http://hz.zhengqikj.top/gtaooighmj.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.xinyue.icu/gtigqbbsjs.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.cucudq.cn/gtyucnllnk.html

[Q61] 移动平均
来源：http://hz.nwbrower.top/gtugddnsuo.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.sufxvd.cn/gtwrzegton.html

[Q62] 分组占比
来源：http://hz.hysaishi.cn/gtdftngwtn.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.zhixingplan.top/gtwybsjcnx.html

[Q63] 开启事务
来源：http://hz.jyoumei.cn/gtlywccznt.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.smart0.xyz/gttszkwdfi.html

[Q64] 提交事务
来源：http://hz.tian-w.cn/gtyiawkzbv.html

COMMIT;
来源：http://hz.zhengqikj.top/gtxervtqwa.html

[Q65] 回滚事务
来源：http://hz.yuanzhike.top/gtbggkchwc.html

ROLLBACK;
来源：http://hz.tanke756.top/gtbxtyupuc.html

[Q66] 行锁查询
来源：http://hz.xuetiantiany.cn/gtusvbfutp.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.chenlongwang.top/gtaomffyoa.html

[Q67] 设置隔离级别
来源：http://hz.zhoulong.xyz/gtkttylycc.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.jyoumei.cn/gtvhmahkza.html

[Q68] 保存点
来源：http://hz.ydjk.org.cn/gtxtgfaqdc.html

SAVEPOINT sp1;
来源：http://hz.0kj1m.cn/gthywiysaa.html

ROLLBACK TO sp1;
来源：http://hz.sxryk.cn/gtishpvjix.html

[Q69] 查看执行计划
来源：http://hz.dianchejie.cn/gtfxbvqqgs.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.zhoulong.xyz/gtplwksbfz.html

[Q70] 更新统计信息
来源：http://hz.tanke756.top/gtkstvxsmb.html

ANALYZE TABLE users;
来源：http://hz.shanyushiyangtech.top/gttarzpvsa.html

[Q71] 查看建表语句
来源：http://hz.fzhhl.top/gtqxieuvfj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.hnxiangtu.top/gtuxggeawc.html

[Q72] 查看索引
来源：http://hz.dashuyun.cn/gtxllqxeya.html

SHOW INDEX FROM users;
来源：http://hz.hysaishi.cn/gteetfbzne.html

[Q73] 查看表状态
来源：http://hz.nanxuanxn.top/gtxgkgfyln.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.hammf.cn/gtmrankyce.html

[Q74] 强制使用索引
来源：http://hz.0kj1m.cn/gtwtfyjpma.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.shanyushiyangtech.top/gttbfqtrjg.html

[Q75] 日期格式化
来源：http://hz.yueranfly.top/gtwnbscpmh.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.fengsongda.top/gtupdigwih.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.feifeiyinyue.top/gtffmefbsn.html

[Q76] 按天统计
来源：http://hz.ybcxt.top/gtnwbsosgv.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.chenzaomai.com/gtyjccgxxq.html

[Q77] 时间加减
来源：http://hz.andypj.xyz/gtrjtuhiay.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.0kj1m.cn/gtwjjfpnjd.html

[Q78] 当前时间
来源：http://hz.feifeiyinyue.top/gtujbiurzn.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.c1oappe.top/gtwcmjsebo.html

[Q79] 字符串拼接
来源：http://hz.hnxiangtu.top/gtuigtxthb.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.hongshengwenyu.top/gtkriktgkw.html

[Q80] 字符串截取
来源：http://hz.ydjk.org.cn/gtynvxfqkb.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.tianlin.xyz/gtdefxxpjc.html

[Q81] 字符串替换
来源：http://hz.zhiwuduotai.top/gtdvpmnmrw.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.hongshengwenyu.top/gtiofxupxq.html

[Q82] 字符长度与字节长度
来源：http://hz.chenjidiqi.icu/gtayrqknil.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.nwbrower.top/gtrduzkcii.html

[Q83] 大小写转换
来源：http://hz.yuanzhike.top/gtgiwgbloe.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.hysaishi.cn/gtckoriaeg.html

[Q84] 去除首尾空格
来源：http://hz.chenzaomai.com/gteqekosiz.html

SELECT TRIM(name) FROM users;
来源：http://hz.meibo888.top/gtwylxavgi.html

[Q85] 数值取整
来源：http://hz.zhoulong.xyz/gtcyxlyisp.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.ydzc1.top/gtqcwrqore.html

[Q86] 读取 JSON 字段
来源：http://hz.jinqigfzy.top/gttqbciqus.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.zhixingplan.top/gtnonxnszl.html

[Q87] JSON 字段做条件
来源：http://hz.ehwqpu.com/gtqikdjwtg.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.zhengqikj.top/gtukdbhsue.html

[Q88] 行转列（条件聚合）
来源：http://hz.fengsongda.top/gtijjweohi.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.cucudq.cn/gtpoajtkwg.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.yanxiufei.cn/gtfzobpytn.html

[Q89] 判断表是否存在
来源：http://hz.yueranfly.top/gtqpkpavds.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.hnxiangtu.top/gtzanekpcs.html

[Q90] 生成序号列
来源：http://hz.zhiwuduotai.top/gtdzamazdp.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.fengsongda.top/gttbkejssa.html

================================================================================
来源：http://hz.316326.xyz/gtcdmlwpfh.html

R. Bash 专题
来源：http://hz.ywan-chungtsiang.top/gtybsjgfsm.html

================================================================================
来源：http://hz.jqgufenzy.top/gtsslcvdht.html

[R01] shebang 与严格模式
来源：http://hz.cucudq.cn/gtfjhbupff.html

#!/usr/bin/env bash
来源：http://hz.chenjidiqi.icu/gtckqxylsr.html

set -euo pipefail
来源：http://hz.52xcode.cn/gtsblespok.html

[R02] 变量赋值与使用
来源：http://hz.gogol.net.cn/gtyctkhmpt.html

name="Tom"; echo "$name"
来源：http://hz.shuidangran.top/gtbazvktpz.html

[R03] 只读变量
来源：http://hz.redwolf501.top/gtvzorcxax.html

readonly PI=3.14
来源：http://hz.chenzaomai.com/gtfptmftaa.html

[R04] 位置参数
来源：http://hz.hnxiangtu.top/gtwxryieaw.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.dianchejie.cn/gtomjbiocv.html

[R05] 参数默认值
来源：http://hz.nanxinkj.top/gtuzcesgjw.html

name="${1:-default}"
来源：http://hz.zhoulong.xyz/gtwvqrldzc.html

[R06] 判断命令是否存在
来源：http://hz.andypj.xyz/gtfqflawmz.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.hywenlv.cn/gtdsgufksc.html

[R07] if 判断文件
来源：http://hz.shanyushiyangkeji.top/gtradbanqr.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.fengsongda.top/gtztncdguc.html

[R08] 数值比较
来源：http://hz.chenjidiqi.icu/gtpcbzajfi.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.hysaishi.cn/gtcniskacv.html

[R09] 字符串比较
来源：http://hz.vqdsnc.cn/gttlrooczc.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.andypj.xyz/gthchqedyr.html

[R10] 正则匹配
来源：http://hz.ybcxt.top/gtazmfxcyl.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.yongpay.top/gtgmuhlxck.html

[R11] case 多分支
来源：http://hz.zhengqikj.top/gtgihwfvmu.html

case "$1" in
来源：http://hz.9152youxi.cn/gtznevvktd.html

start) echo "启动" ;;
来源：http://hz.hywenlv.cn/gtdwnkdeho.html

stop)  echo "停止" ;;
来源：http://hz.cheryme.top/gtlbwectun.html

*)     echo "未知命令" ;;
来源：http://hz.hnxiangtu.top/gteowudamw.html

esac
来源：http://hz.smart0.xyz/gtrwitclwt.html

[R12] for 遍历文件
来源：http://hz.mhx1999.top/gtreawxxow.html

for f in *.txt; do echo "$f"; done
来源：http://hz.chenzaomai.com/gtgbikulyz.html

[R13] for 计数循环
来源：http://hz.haohaochexian.top/gtptllqmxi.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.yueranfly.top/gtvobdeidh.html

[R14] C 风格 for
来源：http://hz.yj202588.top/gttoishzmr.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.yangfankeji.com/gtclypkskq.html

[R15] while 逐行读文件
来源：http://hz.birdmap.top/gtwwjpmutu.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.xylfe.cn/gtqdvihcwf.html

[R16] until 等待条件
来源：http://hz.ehwqpu.com/gttxstygpz.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.9152youxi.cn/gteznwashv.html

[R17] 数组定义与取值
来源：http://hz.xuetiantiany.cn/gtqjrslwts.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.gogol.net.cn/gtvvtqwmdw.html

[R18] 遍历数组
来源：http://hz.tanke756.top/gtlqcytpcc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.yuanzhike.top/gtknakjgeb.html

[R19] 数组长度
来源：http://hz.feifeiyinyue.top/gtwnpirwoe.html

echo "${#arr[@]}"
来源：http://hz.redwolf501.top/gtktodjhru.html

[R20] 关联数组（字典）
来源：http://hz.yj202588.top/gtziemkvbz.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.0kj1m.cn/gtxhtwlghg.html

[R21] 字符串长度
来源：http://hz.yj20258888.top/gtowsjzfld.html

echo "${#s}"
来源：http://hz.wangshuangyany.cn/gtimpmvzsp.html

[R22] 截取子串
来源：http://hz.xuetiantiany.cn/gtxcnxckfy.html

echo "${s:0:5}"
来源：http://hz.c1oappe.top/gtbvgcdbyw.html

[R23] 字符串替换
来源：http://hz.pycfn.com/gthomgfjpm.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.hnxiangtu.top/gtjkyjhlqi.html

[R24] 大小写转换
来源：http://hz.ywan-chungtsiang.top/gtfkikkcvs.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.0kj1m.cn/gtobchvfzr.html

[R25] 去后缀 / 去前缀
来源：http://hz.svipenyu.cn/gtgrnglqio.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.guowangkeji.top/gtkhjcdkxs.html

[R26] 命令替换
来源：http://hz.smart0.xyz/gtwdhbjpkg.html

now=$(date +%F); echo "$now"
来源：http://hz.quarkkingdee.top/gtjzphyocv.html

[R27] 算术展开
来源：http://hz.hnxiangtu.top/gtzmksmzdn.html

echo $((1 + 2 * 3))
来源：http://hz.gzhubu.top/gtlcdmxakr.html

[R28] 浮点运算
来源：http://hz.nanxuanxn.top/gtuiwfpnda.html

echo "scale=2; 10/3" | bc
来源：http://hz.hywenlv.cn/gtumegewyl.html

[R29] 定义函数
来源：http://hz.shanyushiyangkeji.top/gthuirdcow.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.zhiwuduotai.top/gtoltmtuhg.html

[R30] 函数返回状态码
来源：http://hz.dashuyun.cn/gtwudojaem.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.gaohongyu789.top/gtbdjdyzyq.html

[R31] 局部变量
来源：http://hz.yvedp.cn/gtgkmmgubv.html

f() { local x=1; echo "$x"; }
来源：http://hz.chenjidiqi.icu/gtczbdjgvr.html

[R32] 参数个数校验
来源：http://hz.yonumen.top/gtsgpvhevh.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.chenjidiqi.icu/gtqshxhtxh.html

[R33] 捕获错误并提示行号
来源：http://hz.quarkkingdee.top/gtjnmdkdld.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.9152youxi.cn/gtdhkhkdxw.html

[R34] 退出时清理
来源：http://hz.kuanghao11.cn/gtsjdtnurp.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.yvedp.cn/gtlrvrqxvw.html

[R35] 后台执行并等待
来源：http://hz.iojbl.cn/gttjmdsjfg.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.ywan-chungtsiang.top/gttlixvhwt.html

[R36] 并发执行多个任务
来源：http://hz.zdqjudy.top/gttkpnuvte.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.meibo888.top/gtczxzkgvp.html

[R37] 把输出赋给变量
来源：http://hz.jyoumei.cn/gtiydteqvl.html

files=$(ls -1)
来源：http://hz.jqgufenzy.top/gtpwilytqo.html

[R38] 管道串联
来源：http://hz.hysaishi.cn/gtwjarkfet.html

cat a.txt | grep -i error | wc -l
来源：http://hz.pycfn.com/gtckwvirwc.html

[R39] 重定向标准输出与错误
来源：http://hz.hnqzz.top/gtomitquzi.html

cmd > out.log 2>&1
来源：http://hz.hywenlv.cn/gtxsjlewrb.html

[R40] 追加写日志
来源：http://hz.zycfv.cn/gttxrgzkbd.html

echo "log" >> out.log
来源：http://hz.cashguo.top/gttrwnbsmw.html

[R41] 丢弃输出
来源：http://hz.hfpthk.cn/gtvdxjpaew.html

cmd >/dev/null 2>&1
来源：http://hz.hammf.cn/gtipryjvwo.html

[R42] 输入重定向
来源：http://hz.cashguo.top/gtxxalxebe.html

wc -l < a.txt
来源：http://hz.jqgfzy.top/gtvxrlbgah.html

[R43] 按名字查找文件
来源：http://hz.yueranfly.top/gtotbbzapg.html

find . -name "*.log" -type f
来源：http://hz.meibo888.top/gtxmnvabqu.html

[R44] 按修改时间查找
来源：http://hz.chenjidiqi.icu/gtdguebppc.html

find . -mtime -7 -type f
来源：http://hz.sweek.top/gtlbogndbd.html

[R45] 批量删除
来源：http://hz.jianghu66.top/gtitzheaqh.html

find . -name "*.tmp" -delete
来源：http://hz.tanke756.top/gtsjhiyrwi.html

[R46] 递归替换文件内容
来源：http://hz.dianchejie.cn/gtklhfpzcz.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.zhoulong.xyz/gtdrhvidhb.html

[R47] sed 单行替换
来源：http://hz.mhx1999.top/gtkvjipjux.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.feifeiyinyue.top/gtkpulwhwh.html

[R48] awk 取指定列
来源：http://hz.quarkkingdee.top/gtzztazgap.html

awk '{print $1, $3}' a.txt
来源：http://hz.sweek.top/gtagnwffru.html

[R49] awk 带条件
来源：http://hz.chenjidiqi.icu/gtyndxwygj.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.guowangkeji.top/gttqquztfi.html

[R50] awk 求和
来源：http://hz.kuanghao11.cn/gtvcwlhjju.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.ehwqpu.com/gtdilgjvgp.html

[R51] 排序去重取前几
来源：http://hz.sysykeji.top/gtfhqlanmd.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.nwbrower.top/gtkjyjknnu.html

[R52] 统计行数
来源：http://hz.ivvv.top/gtonpjokrx.html

wc -l a.txt
来源：http://hz.yangfankeji.com/gtgyybpkhc.html

[R53] 查看文件头与实时尾
来源：http://hz.shanyushiyangtech.top/gtylhxvdxe.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.cqqwz.cn/gtppabvqjs.html

[R54] 比较两个文件
来源：http://hz.dashuyun.cn/gtmpvylqox.html

diff a.txt b.txt
来源：http://hz.shuidangran.top/gtkbzkoagu.html

[R55] 压缩与解压
来源：http://hz.yuanzhike.top/gtbdpemcxy.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.sweek.top/gtxrbmrxjv.html

[R56] 远程拷贝
来源：http://hz.yj20258.top/gtqdswwryd.html

scp file user@host:/path/
来源：http://hz.yuanzhike.top/gtbyatfjgr.html

[R57] 远程执行命令
来源：http://hz.yuanzhike.top/gtyzpqstuo.html

ssh user@host 'uptime'
来源：http://hz.zhiwuduotai.top/gtbwhoafor.html

[R58] 下载文件
来源：http://hz.hnxiangtu.top/gtmehrhrde.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.yj20258888.top/gtmoytmzzz.html

[R59] 发 POST JSON
来源：http://hz.daxiang520.top/gtxphlftum.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.cqqwz.cn/gtcwshmkxj.html

[R60] 只看 HTTP 状态码
来源：http://hz.sxryk.cn/gtrlbqdcau.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.jinyuanbaomall.cn/gtthzfbuee.html

[R61] 磁盘占用
来源：http://hz.fengsongda.top/gtdokuvqjj.html

df -h;  du -sh *
来源：http://hz.nanxinkj.top/gtncuitvyx.html

[R62] 找最占空间的文件
来源：http://hz.cqqwz.cn/gtgnhaawfa.html

du -ah . | sort -rh | head -10
来源：http://hz.zdqjudy.top/gtcocfeies.html

[R63] 内存与进程
来源：http://hz.hfpthk.cn/gtqtdcpiir.html

free -h;  ps aux | grep nginx
来源：http://hz.snrcjt.cn/gtgqgtvbrw.html

[R64] 结束进程
来源：http://hz.jianghu66.top/gtvslghurg.html

kill -9 $(pgrep -f app.py)
来源：http://hz.ydjk.org.cn/gtyluenorl.html

[R65] 查看端口占用
来源：http://hz.jlsjyb.cn/gtzrbncowl.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.wangdashe.top/gtecvfqsfq.html

[R66] 定时任务
来源：http://hz.yj202588.top/gtxodltwuh.html

crontab -e;  crontab -l
来源：http://hz.sweek.top/gtrwcatssi.html

[R67] 生成随机十六进制串
来源：http://hz.gzhubu.top/gtqkiwhsoy.html

openssl rand -hex 16
来源：http://hz.ydjk.org.cn/gtiwavndum.html

[R68] 计算文件校验值
来源：http://hz.yj20258.top/gtynxtefxg.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.yj202588.top/gtyslrzacz.html

[R69] 生成随机密码
来源：http://hz.gotoacloud.top/gtqzsrslss.html

head -c 16 /dev/urandom | base64
来源：http://hz.nanxuanxn.top/gtqdrlhirs.html

[R70] 时间戳与互转
来源：http://hz.cdnleiting.top/gtzgfuodnj.html

date +%s;  date -d @1700000000
来源：http://hz.jianghu66.top/gtvhnjywdl.html

[R71] 日期格式化
来源：http://hz.kuanghao11.cn/gtvzzimbge.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.birdmap.top/gtaeefbdkw.html

[R72] 等待端口就绪
来源：http://hz.aizwys.cn/gtrquzpgej.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.yongpay.top/gtwavpihse.html

[R73] 分割大日志
来源：http://hz.redwolf501.top/gtrhqtizbh.html

split -l 1000 big.log part_
来源：http://hz.xuanzx.com/gtufrzrawh.html

[R74] 批量重命名
来源：http://hz.hongshengwenyu.top/gtklunhcwt.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.ehwqpu.com/gtwfajcmkv.html

[R75] 导出环境变量
来源：http://hz.0kj1m.cn/gtkvugxtxn.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.ydzc1.top/gtginevsbz.html

[R76] 使用临时文件
来源：http://hz.ivvv.top/gtjefnbtrp.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.ydjk.org.cn/gtejxyosxh.html

[R77] 读取用户输入
来源：http://hz.gaohongyu789.top/gtaxgcuvph.html

read -rp "请输入: " ans
来源：http://hz.pengpengdd.cyou/gtswedlnko.html

[R78] 交互式菜单
来源：http://hz.pengpengdd.cyou/gtivkmyavj.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.jianghu66.top/gtcwnhvbav.html

[R79] 解析命令行选项
来源：http://hz.316326.xyz/gtlkwclyry.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.jiagoushi.top/gtkgsiuphu.html

[R80] 查看脚本执行耗时
来源：http://hz.zhiwuduotai.top/gtgzxqixwp.html

time ./run.sh
来源：http://hz.hywenlv.cn/gtgshuxaii.html

================================================================================
来源：http://hz.chenzaomai.com/gtweatzmhg.html

S. C / C++ 专题
来源：http://hz.fzhhl.top/gtzxtwoxic.html

================================================================================
来源：http://hz.nanxinkj.top/gtizzdfrob.html

[S01] C：Hello World
来源：http://hz.cucudq.cn/gtucebvkyv.html

#include <stdio.h>
来源：http://hz.yueranfly.top/gtwyyacumf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.ehwqpu.com/gtcnxyfpyg.html

[S02] C：变量与格式化输出
来源：http://hz.316326.xyz/gtnhefqlzx.html

int a = 10; printf("%d\n", a);
来源：http://hz.zhoulong.xyz/gtmqactpvn.html

[S03] C：读入整数
来源：http://hz.aibaodan.cn/gtkvpltxiy.html

int x; scanf("%d", &x);
来源：http://hz.yuxming.cn/gtwejzkqyx.html

[S04] C：字符串复制
来源：http://hz.cucudq.cn/gtqemxjdpl.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.hnqzz.top/gtltqbzruo.html

[S05] C：字符串长度
来源：http://hz.wangdashe.top/gtgekazfic.html

strlen(s)
来源：http://hz.cdnleiting.top/gtcgxrkfki.html

[S06] C：字符串比较
来源：http://hz.xingfuxueyuan.xyz/gthgbezxnv.html

strcmp(a, b) == 0
来源：http://hz.9152youxi.cn/gtxvnhbeud.html

[S07] C：数组遍历求和
来源：http://hz.yj20258888.top/gtjlicvesf.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.xuanzx.com/gtxieuzeyx.html

[S08] C：动态内存分配与释放
来源：http://hz.ivvv.top/gtjknsydlz.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.xinyue.icu/gtcgpoaslc.html

[S09] C：结构体定义与初始化
来源：http://hz.cucudq.cn/gthlcenobk.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.hnxiangtu.top/gtlcviprfz.html

[S10] C：指针与解引用
来源：http://hz.smart0.xyz/gtimywicjz.html

int *p = &a;  *p = 5;
来源：http://hz.tianlin.xyz/gtoazxmmmh.html

[S11] C：逐行读文件
来源：http://hz.jinqigfzy.top/gteogsghuv.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.yanxiufei.cn/gtmiyzuezy.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.ivvv.top/gtgsmcsrhs.html

fclose(f);
来源：http://hz.52xcode.cn/gtgjfawjhy.html

[S12] C：写文件
来源：http://hz.redwolf501.top/gtsdubhxyf.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.hysaishi.cn/gtboqnlfjf.html

[S13] C：宏定义
来源：http://hz.jqgufenzy.top/gtjpzyfqhh.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.c1oappe.top/gtivclndwn.html

[S14] C：枚举
来源：http://hz.yanxiufei.cn/gtkihjmpzk.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.gaohongyu789.top/gtfmolfumo.html

[S15] C：类型转换
来源：http://hz.havefunace.top/gthsjuqwty.html

(double) a / b
来源：http://hz.gaohongyu789.top/gtuchovekh.html

[S16] C：位操作置位
来源：http://hz.sufxvd.cn/gtaavjzgva.html


<!-- 参考信息 -->