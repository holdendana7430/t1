代发 wailian999

[Q61] 移动平均
来源：http://hz.xuetiantiany.cn/gtwhqramcg.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.yj202588.top/gtlhztisnp.html

[Q62] 分组占比
来源：http://hz.ydjk.org.cn/gtrmzitsco.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.316326.xyz/gtozbesavr.html

[Q63] 开启事务
来源：http://hz.shanyushiyangtech.top/gtfswwvjkd.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.meibo888.top/gtbjyaisor.html

[Q64] 提交事务
来源：http://hz.hammf.cn/gtbdqlfrvo.html

COMMIT;
来源：http://hz.smart0.xyz/gtddfhisib.html

[Q65] 回滚事务
来源：http://hz.shangyingyoupin.top/gtxabjdqnn.html

ROLLBACK;
来源：http://hz.pycfn.com/gtbzzdpxel.html

[Q66] 行锁查询
来源：http://hz.jinghuilouyu.cn/gtxvrltjiz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.yongpay.top/gtutosogif.html

[Q67] 设置隔离级别
来源：http://hz.ehwqpu.com/gtwisrvbfz.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.yvedp.cn/gtbfuyyorn.html

[Q68] 保存点
来源：http://hz.shzxlz.cn/gtkbtlqrli.html

SAVEPOINT sp1;
来源：http://hz.yj20258.top/gtpdietrhx.html

ROLLBACK TO sp1;
来源：http://hz.cqqwz.cn/gtfzwvnciu.html

[Q69] 查看执行计划
来源：http://hz.zhongyouzk.top/gtvrlzspvz.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.zhengqikj.top/gtuoxkjmog.html

[Q70] 更新统计信息
来源：http://hz.yj20258888.top/gtxejotzth.html

ANALYZE TABLE users;
来源：http://hz.hywenlv.cn/gtxpuhewhf.html

[Q71] 查看建表语句
来源：http://hz.hywenlv.cn/gtncntyxll.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.jianghu66.top/gtfhmgxxqr.html

[Q72] 查看索引
来源：http://hz.shuidangran.top/gtxcsejmqq.html

SHOW INDEX FROM users;
来源：http://hz.dashuyun.cn/gtrjsjigmo.html

[Q73] 查看表状态
来源：http://hz.zhiwuduotai.top/gtzzteymld.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.zhiwuduotai.top/gtdaabtwgb.html

[Q74] 强制使用索引
来源：http://hz.gaohongyu789.top/gtoiwspedp.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.chenjidiqi.icu/gtznvnjxlq.html

[Q75] 日期格式化
来源：http://hz.hywenlv.cn/gtyokygptu.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.havefunace.top/gtrjffpikw.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.hnqzz.top/gtpvkmzzen.html

[Q76] 按天统计
来源：http://hz.sufxvd.cn/gtpvyscdmu.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.chenjidiqi.icu/gthphaoonh.html

[Q77] 时间加减
来源：http://hz.iojbl.cn/gthgstyswr.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.zhoulong.xyz/gtmvisyufh.html

[Q78] 当前时间
来源：http://hz.gaohongyu789.top/gttkhxfknm.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.tian-w.cn/gtwabjdvur.html

[Q79] 字符串拼接
来源：http://hz.cqqwz.cn/gtkuyoglkc.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.andypj.xyz/gtevmbhvrq.html

[Q80] 字符串截取
来源：http://hz.xziqi.cn/gtfyhwndtg.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.fengsongda.top/gtpjyziomx.html

[Q81] 字符串替换
来源：http://hz.ppjwa.cn/gtgimclbrj.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.wangshuangyany.cn/gtyhrpthyh.html

[Q82] 字符长度与字节长度
来源：http://hz.aibaodan.cn/gtihielcja.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.smart0.xyz/gtcwutzgqh.html

[Q83] 大小写转换
来源：http://hz.xuanzx.com/gthavgfwgy.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.guowangkeji.top/gtmuajhzmu.html

[Q84] 去除首尾空格
来源：http://hz.hnqzz.top/gtnigfyhwu.html

SELECT TRIM(name) FROM users;
来源：http://hz.feifeiyinyue.top/gtynapupcj.html

[Q85] 数值取整
来源：http://hz.quarkkingdee.top/gtiglyjerr.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.zhongyouzk.top/gtajwmlscv.html

[Q86] 读取 JSON 字段
来源：http://hz.jinqigufen.top/gtndwoecty.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.ppjwa.cn/gttnrmyaxa.html

[Q87] JSON 字段做条件
来源：http://hz.gogol.net.cn/gtcrkqfutm.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.ydzc1.top/gtxsqtbqqe.html

[Q88] 行转列（条件聚合）
来源：http://hz.cqqwz.cn/gtfaoippzf.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.ppjwa.cn/gtrdjcyycv.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.ydjk.org.cn/gtlbawslyt.html

[Q89] 判断表是否存在
来源：http://hz.zhongyouzk.top/gtucnwwalj.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.jyoumei.cn/gtqswunmgr.html

[Q90] 生成序号列
来源：http://hz.hysaishi.cn/gtdfmtoyig.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.yj202588.top/gtacmmrreq.html

================================================================================
来源：http://hz.ybcxt.top/gtffsqetdc.html

R. Bash 专题
来源：http://hz.gzhubu.top/gtmiwhglgu.html

================================================================================
来源：http://hz.jianghu66.top/gteakfertb.html

[R01] shebang 与严格模式
来源：http://hz.jinqigufen.top/gtuuctrzeu.html

#!/usr/bin/env bash
来源：http://hz.shzxlz.cn/gtthhhdlqb.html

set -euo pipefail
来源：http://hz.redwolf501.top/gtfedrarwf.html

[R02] 变量赋值与使用
来源：http://hz.chenjidiqi.icu/gtgdwzrvkw.html

name="Tom"; echo "$name"
来源：http://hz.kuanghao11.cn/gtobmlnzxm.html

[R03] 只读变量
来源：http://hz.ehwqpu.com/gtdrkfzysz.html

readonly PI=3.14
来源：http://hz.ehwqpu.com/gtygnavdhx.html

[R04] 位置参数
来源：http://hz.9152youxi.cn/gteiyinvfv.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.zhaomingkeji.xyz/gtpyfzabmy.html

[R05] 参数默认值
来源：http://hz.ywan-chungtsiang.top/gtccuoqufu.html

name="${1:-default}"
来源：http://hz.zhijiandao.cn/gtbtjinlmy.html

[R06] 判断命令是否存在
来源：http://hz.nanxuanxn.top/gtonuvkeho.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.shanyushiyangtech.top/gtimbrgcgy.html

[R07] if 判断文件
来源：http://hz.ppjwa.cn/gtakiidcfy.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.dianchejie.cn/gtlrnfnbjg.html

[R08] 数值比较
来源：http://hz.jinqigfzy.top/gtjlcryhos.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.yuxming.cn/gtowqsciii.html

[R09] 字符串比较
来源：http://hz.zhijiandao.cn/gtowggjpmx.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.daria6918.cn/gtfsmjwgty.html

[R10] 正则匹配
来源：http://hz.zdqjudy.top/gtynrxgpeu.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.zhixingplan.top/gttwcijzbp.html

[R11] case 多分支
来源：http://hz.jianghu66.top/gtfxqtnepn.html

case "$1" in
来源：http://hz.ydzc1.top/gthmduaeup.html

start) echo "启动" ;;
来源：http://hz.wangshuangyany.cn/gtyztckigv.html

stop)  echo "停止" ;;
来源：http://hz.iojbl.cn/gtpdzmesgi.html

*)     echo "未知命令" ;;
来源：http://hz.yueranfly.top/gtmnxngpqe.html

esac
来源：http://hz.yongpay.top/gtrsognkyx.html

[R12] for 遍历文件
来源：http://hz.zhijiandao.cn/gtsllkdwfq.html

for f in *.txt; do echo "$f"; done
来源：http://hz.gaohongyu789.top/gtvnnpfzzr.html

[R13] for 计数循环
来源：http://hz.yanxiufei.cn/gtpkytagqf.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.nanxinkj.top/gtlqdttbkv.html

[R14] C 风格 for
来源：http://hz.redwolf501.top/gtugcjkmgv.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.shzxlz.cn/gtqyksnwel.html

[R15] while 逐行读文件
来源：http://hz.birdmap.top/gtodcobfra.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.gogol.net.cn/gttguosmri.html

[R16] until 等待条件
来源：http://hz.gzhubu.top/gtmxugadge.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.jqgfzy.top/gtfdzoujtd.html

[R17] 数组定义与取值
来源：http://hz.hnxiangtu.top/gtfqjawcqa.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.yueranfly.top/gtxxasxvrc.html

[R18] 遍历数组
来源：http://hz.316326.xyz/gtwoplzqyc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.dashuyun.cn/gtjttvtpfc.html

[R19] 数组长度
来源：http://hz.andypj.xyz/gtpijvkssx.html

echo "${#arr[@]}"
来源：http://hz.gotoacloud.top/gtfzcxqdvd.html

[R20] 关联数组（字典）
来源：http://hz.quarkkingdee.top/gtznpmqhed.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.smart0.xyz/gteedszxqd.html

[R21] 字符串长度
来源：http://hz.fengsongda.top/gthdyirwae.html

echo "${#s}"
来源：http://hz.bjfxy.top/gthfesvcjj.html

[R22] 截取子串
来源：http://hz.daxiang520.top/gtrlpemivl.html

echo "${s:0:5}"
来源：http://hz.wangdashe.top/gtedfgjjdy.html

[R23] 字符串替换
来源：http://hz.ppjwa.cn/gtqcpbljcp.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.shzxlz.cn/gthizigryu.html

[R24] 大小写转换
来源：http://hz.dianchejie.cn/gttpfcxnxt.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.quarkkingdee.top/gtgtgeaopx.html

[R25] 去后缀 / 去前缀
来源：http://hz.quarkkingdee.top/gtmbgdyutp.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.ywan-chungtsiang.top/gtarphltmk.html

[R26] 命令替换
来源：http://hz.shangyingyoupin.top/gtefmqhant.html

now=$(date +%F); echo "$now"
来源：http://hz.ivvv.top/gtzqekvgjw.html

[R27] 算术展开
来源：http://hz.nanxuanxn.top/gtrxufzegj.html

echo $((1 + 2 * 3))
来源：http://hz.yonumen.top/gtoejxkcse.html

[R28] 浮点运算
来源：http://hz.gogol.net.cn/gtsltswezb.html

echo "scale=2; 10/3" | bc
来源：http://hz.birdmap.top/gtbhdqtthh.html

[R29] 定义函数
来源：http://hz.jinqigufen.top/gttzvivhhu.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.jinqigfzy.top/gtoandivet.html

[R30] 函数返回状态码
来源：http://hz.chenzaomai.com/gtbnalnzft.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.chenlongwang.top/gtzvoynjsr.html

[R31] 局部变量
来源：http://hz.xuanzx.com/gtsaafcpvi.html

f() { local x=1; echo "$x"; }
来源：http://hz.yvedp.cn/gtrljpszht.html

[R32] 参数个数校验
来源：http://hz.shangyingyoupin.top/gtwkgptupw.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.chenjidiqi.icu/gtiettishq.html

[R33] 捕获错误并提示行号
来源：http://hz.wangdashe.top/gteurrsfbw.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.hysaishi.cn/gtnckdypup.html

[R34] 退出时清理
来源：http://hz.sxryk.cn/gtsmhjinlv.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.cheryme.top/gtzexkwywk.html

[R35] 后台执行并等待
来源：http://hz.hnqzz.top/gtgoazvooy.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.meibo888.top/gtqtwtvqxi.html

[R36] 并发执行多个任务
来源：http://hz.aibaodan.cn/gtnebkofwj.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.shanyushiyangkeji.top/gtcpgiyscu.html

[R37] 把输出赋给变量
来源：http://hz.aizwys.cn/gtqsdthtsv.html

files=$(ls -1)
来源：http://hz.sufxvd.cn/gtjfgqhqkp.html

[R38] 管道串联
来源：http://hz.gotoacloud.top/gtwxenxxyv.html

cat a.txt | grep -i error | wc -l
来源：http://hz.shzxlz.cn/gtjzfwwuqs.html

[R39] 重定向标准输出与错误
来源：http://hz.hysaishi.cn/gtsgstfqzx.html

cmd > out.log 2>&1
来源：http://hz.cheryme.top/gtgepvfbuc.html

[R40] 追加写日志
来源：http://hz.chenjidiqi.icu/gtbjtzsfcw.html

echo "log" >> out.log
来源：http://hz.xziqi.cn/gtvxpuikeu.html

[R41] 丢弃输出
来源：http://hz.jianghu66.top/gtckhdvcbb.html

cmd >/dev/null 2>&1
来源：http://hz.tanke756.top/gttdhrdoqh.html

[R42] 输入重定向
来源：http://hz.yj20258.top/gtaoswuejb.html

wc -l < a.txt
来源：http://hz.zhengqikj.top/gtvpcgphhw.html

[R43] 按名字查找文件
来源：http://hz.nanxuanxn.top/gtrpphezyp.html

find . -name "*.log" -type f
来源：http://hz.ydjk.org.cn/gtjpjyzewf.html

[R44] 按修改时间查找
来源：http://hz.yj202588.top/gtfjmdawmn.html

find . -mtime -7 -type f
来源：http://hz.snrcjt.cn/gtdgyzjruc.html

[R45] 批量删除
来源：http://hz.xylfe.cn/gtqesptgqc.html

find . -name "*.tmp" -delete
来源：http://hz.sysykeji.top/gtxtbmoles.html

[R46] 递归替换文件内容
来源：http://hz.c1oappe.top/gtqdnjmmvf.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.xinyue.icu/gtcvzyqbyp.html

[R47] sed 单行替换
来源：http://hz.daria6918.cn/gtupwfljjq.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.ybcxt.top/gtygddqtpy.html

[R48] awk 取指定列
来源：http://hz.zhijiandao.cn/gtfauoebfa.html

awk '{print $1, $3}' a.txt
来源：http://hz.iojbl.cn/gtwkkggfej.html

[R49] awk 带条件
来源：http://hz.xuanzx.com/gtzufqbqnq.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.zhixingplan.top/gtyvwoemuv.html

[R50] awk 求和
来源：http://hz.daxiang520.top/gtalhsongw.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.jianghu66.top/gtohnzuusd.html

[R51] 排序去重取前几
来源：http://hz.yangfankeji.com/gtpvdxnofw.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.yj202588.top/gtlahvbmnt.html

[R52] 统计行数
来源：http://hz.chenlongwang.top/gtipyfhugo.html

wc -l a.txt
来源：http://hz.jinqigufen.top/gtykxmqrci.html

[R53] 查看文件头与实时尾
来源：http://hz.vqdsnc.cn/gtedugwdmo.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.yongpay.top/gtrhzhzvyn.html

[R54] 比较两个文件
来源：http://hz.0kj1m.cn/gtismtauxf.html

diff a.txt b.txt
来源：http://hz.yj20258888.top/gtapajnnyr.html

[R55] 压缩与解压
来源：http://hz.zhijiandao.cn/gtzhypmzyl.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.yonumen.top/gtpveobnyo.html

[R56] 远程拷贝
来源：http://hz.sysykeji.top/gtqcbtryxm.html

scp file user@host:/path/
来源：http://hz.jlsjyb.cn/gtgdfzmmfw.html

[R57] 远程执行命令
来源：http://hz.zhoulong.xyz/gtikgaykux.html

ssh user@host 'uptime'
来源：http://hz.sysykeji.top/gtiklwznwz.html

[R58] 下载文件
来源：http://hz.shangyingyoupin.top/gtdkbqyagj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.zycfv.cn/gtvezywedb.html

[R59] 发 POST JSON
来源：http://hz.0kj1m.cn/gtynwxsjtg.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yonumen.top/gtibvativc.html

[R60] 只看 HTTP 状态码
来源：http://hz.yangfankeji.com/gtwswgbfff.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.gogol.net.cn/gtvlvglipm.html

[R61] 磁盘占用
来源：http://hz.wangshuangyany.cn/gtetttrlhj.html

df -h;  du -sh *
来源：http://hz.iojbl.cn/gtupelixho.html

[R62] 找最占空间的文件
来源：http://hz.ybcxt.top/gtegfxrwij.html

du -ah . | sort -rh | head -10
来源：http://hz.tanke756.top/gttxfpshdx.html

[R63] 内存与进程
来源：http://hz.fengsongda.top/gtbfakntkg.html

free -h;  ps aux | grep nginx
来源：http://hz.xuanzx.com/gtnmsexgdd.html

[R64] 结束进程
来源：http://hz.xziqi.cn/gtjbvwksrx.html

kill -9 $(pgrep -f app.py)
来源：http://hz.ydzc1.top/gtsxjpzmop.html

[R65] 查看端口占用
来源：http://hz.0kj1m.cn/gtonwotcyh.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.quarkkingdee.top/gtdmcjifly.html

[R66] 定时任务
来源：http://hz.zhoulong.xyz/gtljtttxzc.html

crontab -e;  crontab -l
来源：http://hz.xinyue.icu/gtcfmauvcs.html

[R67] 生成随机十六进制串
来源：http://hz.jqgfzy.top/gtmezpsaxx.html

openssl rand -hex 16
来源：http://hz.nwbrower.top/gtkxhvvxwn.html

[R68] 计算文件校验值
来源：http://hz.zhengqikj.top/gtsytgjnvb.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.smart0.xyz/gtohbtzppf.html

[R69] 生成随机密码
来源：http://hz.hnqzz.top/gtddmwltoq.html

head -c 16 /dev/urandom | base64
来源：http://hz.svipenyu.cn/gtysyshmhu.html

[R70] 时间戳与互转
来源：http://hz.52xcode.cn/gtvbiddesi.html

date +%s;  date -d @1700000000
来源：http://hz.svipenyu.cn/gtlshsdblq.html

[R71] 日期格式化
来源：http://hz.jlsjyb.cn/gtipqugjdt.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.feifeiyinyue.top/gtrubrwify.html

[R72] 等待端口就绪
来源：http://hz.gotoacloud.top/gtstgmsxdq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.zhiwuduotai.top/gteshvjqju.html

[R73] 分割大日志
来源：http://hz.jinyuanbaomall.cn/gtiupwqpup.html

split -l 1000 big.log part_
来源：http://hz.hammf.cn/gtlqaudkns.html

[R74] 批量重命名
来源：http://hz.c1oappe.top/gtcmjyizzi.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.mhx1999.top/gtcerrmvmj.html

[R75] 导出环境变量
来源：http://hz.yvedp.cn/gticmmcmxr.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.pengpengdd.cyou/gtemswtyjz.html

[R76] 使用临时文件
来源：http://hz.fengsongda.top/gtvmaakngg.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.kuanghao11.cn/gtaqrbavoi.html

[R77] 读取用户输入
来源：http://hz.guowangkeji.top/gtfswbqiic.html

read -rp "请输入: " ans
来源：http://hz.guowangkeji.top/gtojwqlhjg.html

[R78] 交互式菜单
来源：http://hz.chenzaomai.com/gtoamblfjp.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.nwbrower.top/gtsqrtsioj.html

[R79] 解析命令行选项
来源：http://hz.sxryk.cn/gtfkrxpkvy.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.jlsjyb.cn/gttzdobfne.html

[R80] 查看脚本执行耗时
来源：http://hz.ppjwa.cn/gteiyubfcf.html

time ./run.sh
来源：http://hz.52xcode.cn/gtnmofzmre.html

================================================================================
来源：http://hz.nanxinkj.top/gtkizobhyh.html

S. C / C++ 专题
来源：http://hz.jinyuanbaomall.cn/gtwazmxmsr.html

================================================================================
来源：http://hz.havefunace.top/gtrvcdsvig.html

[S01] C：Hello World
来源：http://hz.cdnleiting.top/gtsapirjjy.html

#include <stdio.h>
来源：http://hz.guannengcc.top/gtydloehge.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.chenzaomai.com/gtzeuuqwyv.html

[S02] C：变量与格式化输出
来源：http://hz.shzxlz.cn/gtworclysy.html

int a = 10; printf("%d\n", a);
来源：http://hz.cashguo.top/gtduhrdinr.html

[S03] C：读入整数
来源：http://hz.redwolf501.top/gtwxdvoowj.html

int x; scanf("%d", &x);
来源：http://hz.meibo888.top/gtwagtodzu.html

[S04] C：字符串复制
来源：http://hz.zhengqikj.top/gtpzrzpays.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.cheryme.top/gtptclrsuc.html

[S05] C：字符串长度
来源：http://hz.tanke756.top/gtfxlfvpdj.html

strlen(s)
来源：http://hz.xuanzx.com/gtfggfmrbo.html

[S06] C：字符串比较
来源：http://hz.316326.xyz/gtlmtxrmby.html

strcmp(a, b) == 0
来源：http://hz.chenzaomai.com/gtdyujzuxg.html

[S07] C：数组遍历求和
来源：http://hz.guowangkeji.top/gthgkqoydy.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.yanxiufei.cn/gtpiyjltvl.html

[S08] C：动态内存分配与释放
来源：http://hz.shangyingyoupin.top/gtnmmhnska.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.52xcode.cn/gtmesmswnx.html

[S09] C：结构体定义与初始化
来源：http://hz.zhengqikj.top/gtntcianpg.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.chenjidiqi.icu/gttjdslewn.html

[S10] C：指针与解引用
来源：http://hz.fengsongda.top/gtnnybdoky.html

int *p = &a;  *p = 5;
来源：http://hz.jyoumei.cn/gtkwygyaka.html

[S11] C：逐行读文件
来源：http://hz.hongshengwenyu.top/gtefnrdeea.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.birdmap.top/gticemqqcj.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.hfpthk.cn/gtjkrqkakn.html

fclose(f);
来源：http://hz.yj202588.top/gtagyldmbg.html

[S12] C：写文件
来源：http://hz.jyoumei.cn/gtmtinbuzd.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.chenjidiqi.icu/gtkrksudlj.html

[S13] C：宏定义
来源：http://hz.wangshuangyany.cn/gtghleokgn.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.smart0.xyz/gtpyddxvbg.html

[S14] C：枚举
来源：http://hz.xingfuxueyuan.xyz/gtvqbjromc.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.hongshengwenyu.top/gtgytojurw.html

[S15] C：类型转换
来源：http://hz.aibaodan.cn/gtxrtxgutz.html

(double) a / b
来源：http://hz.sxryk.cn/gtogrvbhnf.html

[S16] C：位操作置位
来源：http://hz.xziqi.cn/gtgkyvhcch.html

x |= (1 << 3);
来源：http://hz.sysykeji.top/gtrihntdcq.html

[S17] C：安全拼接字符串
来源：http://hz.hywenlv.cn/gtpydfbbyi.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.mhx1999.top/gtpwezebde.html

[S18] C：命令行参数
来源：http://hz.hammf.cn/gticgymyqe.html

int main(int argc, char **argv)
来源：http://hz.xingfuxueyuan.xyz/gtjeujsbgk.html

[S19] C：快速排序
来源：http://hz.yuxming.cn/gtznhkjahe.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.dashuyun.cn/gtxvailqzo.html

[S20] C：二分查找
来源：http://hz.nanxinkj.top/gtqalnxvbw.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.yanxiufei.cn/gtpcbtsoqx.html

[S21] C：字符类别判断
来源：http://hz.shangyingyoupin.top/gtshmrxtqe.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.hysaishi.cn/gtbkclsrod.html

[S22] C：字符串转数字
来源：http://hz.shanyushiyangkeji.top/gteqhcdzod.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.smart0.xyz/gtwrggciln.html

[S23] C：随机数
来源：http://hz.jinqigfzy.top/gtspzwldmm.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.jinghuilouyu.cn/gtfqjhhyfq.html

[S24] C：获取本地时间
来源：http://hz.andypj.xyz/gtkosyvhky.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.hongshengwenyu.top/gtadrepxtn.html

[S25] C：内存拷贝
来源：http://hz.c1oappe.top/gtobpwvioe.html

memcpy(dst, src, n);
来源：http://hz.aibaodan.cn/gtxlvvfiqs.html

[S26] C：内存清零
来源：http://hz.feifeiyinyue.top/gtiebbnkap.html

memset(a, 0, sizeof a);
来源：http://hz.xinyue.icu/gtpwqskasd.html

[S27] C：定义常量
来源：http://hz.shanyushiyangtech.top/gtepgqhqaq.html

const double PI = 3.14159;
来源：http://hz.xuanzx.com/gtfflvgzvw.html

[S28] C：静态变量
来源：http://hz.jinghuilouyu.cn/gtvivpjcpu.html

static int counter = 0;
来源：http://hz.ybcxt.top/gtjzfsirrd.html

[S29] C：变参函数
来源：http://hz.cheryme.top/gtyecdkolp.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.snrcjt.cn/gtqvxymrex.html

[S30] C：头文件保护
来源：http://hz.yj202588.top/gttdgldazk.html

#ifndef X_H
来源：http://hz.yonumen.top/gtdzlzomao.html

#define X_H
来源：http://hz.zhixingplan.top/gtsfjuaiwc.html

#endif
来源：http://hz.0kj1m.cn/gtdhllbkyp.html

[S31] C++：Hello World
来源：http://hz.9152youxi.cn/gtsxqovxga.html


<!-- 参考信息 -->