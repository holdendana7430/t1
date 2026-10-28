代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.shanyushiyangkeji.top/gtdfvvsqki.html

[Q60] 取上一行 / 下一行
来源：http://hz.yongpay.top/gtapbxvkpy.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.jlsjyb.cn/gttzczepwq.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.ppjwa.cn/gtttvoaary.html

[Q61] 移动平均
来源：http://hz.xingfuxueyuan.xyz/gtdntoyanv.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.quarkkingdee.top/gtdzqctocf.html

[Q62] 分组占比
来源：http://hz.cdnleiting.top/gtmsujvzjf.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.vqdsnc.cn/gtfzxjyjtc.html

[Q63] 开启事务
来源：http://hz.yongpay.top/gtabiztupx.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.zhongyouzk.top/gtjiqzddfv.html

[Q64] 提交事务
来源：http://hz.zhongyouzk.top/gtflqknqgw.html

COMMIT;
来源：http://hz.xziqi.cn/gtoisaktcr.html

[Q65] 回滚事务
来源：http://hz.daxiang520.top/gtbmmniryz.html

ROLLBACK;
来源：http://hz.0kj1m.cn/gtmvmozabw.html

[Q66] 行锁查询
来源：http://hz.jqgufenzy.top/gtkohxijjz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.nwbrower.top/gtjlcqxfzj.html

[Q67] 设置隔离级别
来源：http://hz.tianlin.xyz/gtqcdchzds.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.ydjk.org.cn/gtngmjyvew.html

[Q68] 保存点
来源：http://hz.ywan-chungtsiang.top/gtlegqktcd.html

SAVEPOINT sp1;
来源：http://hz.xziqi.cn/gtpjxebklb.html

ROLLBACK TO sp1;
来源：http://hz.0kj1m.cn/gtqfejvcfn.html

[Q69] 查看执行计划
来源：http://hz.xuetiantiany.cn/gtqokwjlbb.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.meibo888.top/gtszcoxjrs.html

[Q70] 更新统计信息
来源：http://hz.chenzaomai.com/gtetqpmzcj.html

ANALYZE TABLE users;
来源：http://hz.yongpay.top/gtwadelbzu.html

[Q71] 查看建表语句
来源：http://hz.tanke756.top/gtursqppfg.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.nanxuanxn.top/gtjxfyyxnv.html

[Q72] 查看索引
来源：http://hz.cqqwz.cn/gtehvvamcc.html

SHOW INDEX FROM users;
来源：http://hz.xuanzx.com/gtqzzdbhpa.html

[Q73] 查看表状态
来源：http://hz.sysykeji.top/gtvgbvrtox.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.zhoulong.xyz/gtxbxqfyrx.html

[Q74] 强制使用索引
来源：http://hz.aibaodan.cn/gtdcmgkgsx.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.hywenlv.cn/gtltlpdypg.html

[Q75] 日期格式化
来源：http://hz.daxiang520.top/gtubowtbie.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.cdnleiting.top/gtrcaadkjn.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.ydzc1.top/gtsbprcirt.html

[Q76] 按天统计
来源：http://hz.guannengcc.top/gtculpbvzz.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.haohaochexian.top/gtpogwkjzh.html

[Q77] 时间加减
来源：http://hz.c1oappe.top/gtvngkgwbr.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.jlsjyb.cn/gtzncfdqvp.html

[Q78] 当前时间
来源：http://hz.hnxiangtu.top/gtsusnqbqg.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.yvedp.cn/gtqhxglnto.html

[Q79] 字符串拼接
来源：http://hz.feifeiyinyue.top/gtoolmsavt.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.guannengcc.top/gtzwomkcmw.html

[Q80] 字符串截取
来源：http://hz.tianlin.xyz/gtoyvcnqdw.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.hammf.cn/gtoprtuhhn.html

[Q81] 字符串替换
来源：http://hz.yonumen.top/gtjtjwqaxs.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.hnqzz.top/gtvcvvvstu.html

[Q82] 字符长度与字节长度
来源：http://hz.bjfxy.top/gtgjaiuhzr.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.xuanzx.com/gtufjdscfo.html

[Q83] 大小写转换
来源：http://hz.chenlongwang.top/gtirhhxvqu.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.daxiang520.top/gteodbnfel.html

[Q84] 去除首尾空格
来源：http://hz.zhengqikj.top/gteawugxsk.html

SELECT TRIM(name) FROM users;
来源：http://hz.yuxming.cn/gtaqdznpbl.html

[Q85] 数值取整
来源：http://hz.9152youxi.cn/gtbptcnozo.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.gotoacloud.top/gtyrmpavxw.html

[Q86] 读取 JSON 字段
来源：http://hz.ivvv.top/gtshwfmdxj.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.yonumen.top/gtroqwqtwk.html

[Q87] JSON 字段做条件
来源：http://hz.nwbrower.top/gttnaivrcj.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.yongpay.top/gtmaegoaxg.html

[Q88] 行转列（条件聚合）
来源：http://hz.wangshuangyany.cn/gtrovvtost.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.hammf.cn/gtjcnrbkax.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.pengpengdd.cyou/gtbnhvvlnz.html

[Q89] 判断表是否存在
来源：http://hz.mhx1999.top/gtrnydzfsh.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.yueranfly.top/gtvcgivjcs.html

[Q90] 生成序号列
来源：http://hz.birdmap.top/gtlwvdshsb.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.kuanghao11.cn/gtrefqitgn.html

================================================================================
来源：http://hz.jinqigfzy.top/gtgdqrqgpa.html

R. Bash 专题
来源：http://hz.ydjk.org.cn/gtunfoixbg.html

================================================================================
来源：http://hz.sufxvd.cn/gtccsbqesr.html

[R01] shebang 与严格模式
来源：http://hz.xinyue.icu/gtywkpomos.html

#!/usr/bin/env bash
来源：http://hz.aizwys.cn/gtrpqflybd.html

set -euo pipefail
来源：http://hz.havefunace.top/gtncksgczw.html

[R02] 变量赋值与使用
来源：http://hz.zhoulong.xyz/gthpaqhpww.html

name="Tom"; echo "$name"
来源：http://hz.ppjwa.cn/gtzfnpfuhz.html

[R03] 只读变量
来源：http://hz.gzhubu.top/gtxaqutosf.html

readonly PI=3.14
来源：http://hz.hywenlv.cn/gtogwcfdfr.html

[R04] 位置参数
来源：http://hz.xinyue.icu/gttjtbsbji.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.fzhhl.top/gtfcrqqcej.html

[R05] 参数默认值
来源：http://hz.fengsongda.top/gtvluijiai.html

name="${1:-default}"
来源：http://hz.zhaomingkeji.xyz/gtqticgdqm.html

[R06] 判断命令是否存在
来源：http://hz.shangyingyoupin.top/gtxwdtgppb.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.xuanzx.com/gtikgkqffg.html

[R07] if 判断文件
来源：http://hz.pengpengdd.cyou/gtoslpdbdh.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.zhaomingkeji.xyz/gtozlbilqi.html

[R08] 数值比较
来源：http://hz.chenzaomai.com/gtusfmjhse.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.tianlin.xyz/gtdximvefh.html

[R09] 字符串比较
来源：http://hz.jinyuanbaomall.cn/gtenrknpmc.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.gogol.net.cn/gttwsenude.html

[R10] 正则匹配
来源：http://hz.hnqzz.top/gtekvdbplu.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.iojbl.cn/gtroqyvzqr.html

[R11] case 多分支
来源：http://hz.xingfuxueyuan.xyz/gtoqnpqtga.html

case "$1" in
来源：http://hz.shanyushiyangtech.top/gtqpvnfyrp.html

start) echo "启动" ;;
来源：http://hz.quarkkingdee.top/gtqzixtngd.html

stop)  echo "停止" ;;
来源：http://hz.daxiang520.top/gtfmxbtfac.html

*)     echo "未知命令" ;;
来源：http://hz.jlsjyb.cn/gtavmqmswg.html

esac
来源：http://hz.jinyuanbaomall.cn/gtwhhoqylk.html

[R12] for 遍历文件
来源：http://hz.tianlin.xyz/gtvedhthiv.html

for f in *.txt; do echo "$f"; done
来源：http://hz.sxryk.cn/gthnqyakcm.html

[R13] for 计数循环
来源：http://hz.jinqigfzy.top/gtvogxnhnt.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.52xcode.cn/gtknxhmtgp.html

[R14] C 风格 for
来源：http://hz.ybcxt.top/gtauhtendd.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.hywenlv.cn/gtpfvbmqvv.html

[R15] while 逐行读文件
来源：http://hz.jqgufenzy.top/gtiylyqdxq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.fzhhl.top/gtvuwjrzqa.html

[R16] until 等待条件
来源：http://hz.sxryk.cn/gtkxanerfd.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.vqdsnc.cn/gtytbqqccd.html

[R17] 数组定义与取值
来源：http://hz.andypj.xyz/gtjknbguwk.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.shanyushiyangtech.top/gtpdvpjwyx.html

[R18] 遍历数组
来源：http://hz.nanxinkj.top/gtngotjmda.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.feifeiyinyue.top/gtnxhdeqxg.html

[R19] 数组长度
来源：http://hz.yuanzhike.top/gtczgylecl.html

echo "${#arr[@]}"
来源：http://hz.hongshengwenyu.top/gtfkgwsxpu.html

[R20] 关联数组（字典）
来源：http://hz.yj20258888.top/gthskfwppk.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.zhijiandao.cn/gttnzeoohd.html

[R21] 字符串长度
来源：http://hz.quarkkingdee.top/gtmorwcehs.html

echo "${#s}"
来源：http://hz.yuanzhike.top/gtwsnskpol.html

[R22] 截取子串
来源：http://hz.vqdsnc.cn/gtatvdfwjr.html

echo "${s:0:5}"
来源：http://hz.cashguo.top/gtswxampav.html

[R23] 字符串替换
来源：http://hz.hfpthk.cn/gtugailqpw.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.jinyuanbaomall.cn/gtyeaxcbur.html

[R24] 大小写转换
来源：http://hz.52xcode.cn/gtzezslsns.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.zhoulong.xyz/gtodkthwlw.html

[R25] 去后缀 / 去前缀
来源：http://hz.c1oappe.top/gtddvulpxh.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.zdqjudy.top/gtknqxaznm.html

[R26] 命令替换
来源：http://hz.meibo888.top/gtdodnepri.html

now=$(date +%F); echo "$now"
来源：http://hz.52xcode.cn/gtifdzufhz.html

[R27] 算术展开
来源：http://hz.dianchejie.cn/gtwfmmfhkp.html

echo $((1 + 2 * 3))
来源：http://hz.yuxming.cn/gtpgbetecl.html

[R28] 浮点运算
来源：http://hz.xingfuxueyuan.xyz/gtjstufkma.html

echo "scale=2; 10/3" | bc
来源：http://hz.zycfv.cn/gtlrlqafiy.html

[R29] 定义函数
来源：http://hz.jinghuilouyu.cn/gtamnqojsr.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.shzxlz.cn/gtryinzyoi.html

[R30] 函数返回状态码
来源：http://hz.hywenlv.cn/gtboiwtbbb.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.hfpthk.cn/gtpdaqozuc.html

[R31] 局部变量
来源：http://hz.pengpengdd.cyou/gtenzyfhgr.html

f() { local x=1; echo "$x"; }
来源：http://hz.fzhhl.top/gthhcfygxg.html

[R32] 参数个数校验
来源：http://hz.cashguo.top/gtvcyqchgx.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.jinghuilouyu.cn/gtehxklrfl.html

[R33] 捕获错误并提示行号
来源：http://hz.xylfe.cn/gtpnnhaufx.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.mhx1999.top/gtczvzrmny.html

[R34] 退出时清理
来源：http://hz.jinghuilouyu.cn/gtkmononfi.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.xuanzx.com/gtjygruqlz.html

[R35] 后台执行并等待
来源：http://hz.cqqwz.cn/gtlyutpdck.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.chenlongwang.top/gturcjwfio.html

[R36] 并发执行多个任务
来源：http://hz.ppjwa.cn/gtqoaaefim.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.zhiwuduotai.top/gtrpcgzwzg.html

[R37] 把输出赋给变量
来源：http://hz.havefunace.top/gthtgulmmh.html

files=$(ls -1)
来源：http://hz.cqqwz.cn/gtnnkxudhw.html

[R38] 管道串联
来源：http://hz.sweek.top/gtonczshrs.html

cat a.txt | grep -i error | wc -l
来源：http://hz.feifeiyinyue.top/gtofgdojyl.html

[R39] 重定向标准输出与错误
来源：http://hz.hywenlv.cn/gtucfuttov.html

cmd > out.log 2>&1
来源：http://hz.havefunace.top/gtjfbxzntu.html

[R40] 追加写日志
来源：http://hz.sysykeji.top/gtnegrxxmc.html

echo "log" >> out.log
来源：http://hz.zhoulong.xyz/gtwclhzkcy.html

[R41] 丢弃输出
来源：http://hz.hongshengwenyu.top/gtphbokpui.html

cmd >/dev/null 2>&1
来源：http://hz.jqgfzy.top/gtchjzeuud.html

[R42] 输入重定向
来源：http://hz.ydjk.org.cn/gtupruyyjr.html

wc -l < a.txt
来源：http://hz.aizwys.cn/gtoshyxpkk.html

[R43] 按名字查找文件
来源：http://hz.cashguo.top/gtofraczmy.html

find . -name "*.log" -type f
来源：http://hz.yuanzhike.top/gtpdtwljrd.html

[R44] 按修改时间查找
来源：http://hz.hongshengwenyu.top/gtjixzkhud.html

find . -mtime -7 -type f
来源：http://hz.sysykeji.top/gtnvfzurrs.html

[R45] 批量删除
来源：http://hz.yj202588.top/gthzvtvmul.html

find . -name "*.tmp" -delete
来源：http://hz.birdmap.top/gtlchfbtdo.html

[R46] 递归替换文件内容
来源：http://hz.gaohongyu789.top/gtjqxvtufu.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.nanxinkj.top/gtoewyhjhx.html

[R47] sed 单行替换
来源：http://hz.yanxiufei.cn/gtlvajjyqq.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.xziqi.cn/gtcbgpyigt.html

[R48] awk 取指定列
来源：http://hz.ydzc1.top/gtbbzevrsq.html

awk '{print $1, $3}' a.txt
来源：http://hz.shanyushiyangkeji.top/gtschyrrfc.html

[R49] awk 带条件
来源：http://hz.jinqigfzy.top/gtbsavunoj.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.hysaishi.cn/gtjljphvlh.html

[R50] awk 求和
来源：http://hz.gaohongyu789.top/gtbbazdbll.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.jqgfzy.top/gtlqumztor.html

[R51] 排序去重取前几
来源：http://hz.jinyuanbaomall.cn/gtniojwlba.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.cheryme.top/gtmmexdqdn.html

[R52] 统计行数
来源：http://hz.yangfankeji.com/gtxrkxffcq.html

wc -l a.txt
来源：http://hz.sweek.top/gtqamulfil.html

[R53] 查看文件头与实时尾
来源：http://hz.yongpay.top/gtvlnufufd.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.xziqi.cn/gtahpjeuag.html

[R54] 比较两个文件
来源：http://hz.daria6918.cn/gtewzyptwf.html

diff a.txt b.txt
来源：http://hz.yuxming.cn/gtvqbijphf.html

[R55] 压缩与解压
来源：http://hz.andypj.xyz/gtvfykxqbb.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.cashguo.top/gtnftvhrcs.html

[R56] 远程拷贝
来源：http://hz.jinyuanbaomall.cn/gtppcnumqv.html

scp file user@host:/path/
来源：http://hz.yongpay.top/gtvmudsvqr.html

[R57] 远程执行命令
来源：http://hz.yuxming.cn/gtqecofkwq.html

ssh user@host 'uptime'
来源：http://hz.c1oappe.top/gtgdrspvrf.html

[R58] 下载文件
来源：http://hz.ywan-chungtsiang.top/gtwkkmwtqn.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.zhiwuduotai.top/gtxxsymfsv.html

[R59] 发 POST JSON
来源：http://hz.jinghuilouyu.cn/gtxsyepfyf.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.hysaishi.cn/gtjqxgyrmu.html

[R60] 只看 HTTP 状态码
来源：http://hz.wangdashe.top/gteexzvbna.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.gotoacloud.top/gtyiowjlav.html

[R61] 磁盘占用
来源：http://hz.yj20258.top/gtbzzxzkke.html

df -h;  du -sh *
来源：http://hz.jqgfzy.top/gtzdhsrvfh.html

[R62] 找最占空间的文件
来源：http://hz.jqgufenzy.top/gtdzhmwwoo.html

du -ah . | sort -rh | head -10
来源：http://hz.fzhhl.top/gtndmsntmw.html

[R63] 内存与进程
来源：http://hz.gogol.net.cn/gtfwgurcyy.html

free -h;  ps aux | grep nginx
来源：http://hz.pengpengdd.cyou/gthulrgumn.html

[R64] 结束进程
来源：http://hz.zdqjudy.top/gtnvdybpti.html

kill -9 $(pgrep -f app.py)
来源：http://hz.aibaodan.cn/gtrxjsubkd.html

[R65] 查看端口占用
来源：http://hz.hnqzz.top/gtknxocrik.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.9152youxi.cn/gtewidqduw.html

[R66] 定时任务
来源：http://hz.haohaochexian.top/gtacgtvkxg.html

crontab -e;  crontab -l
来源：http://hz.ybcxt.top/gtrwqldmcs.html

[R67] 生成随机十六进制串
来源：http://hz.chenzaomai.com/gtssirugib.html

openssl rand -hex 16
来源：http://hz.fzhhl.top/gtvtmlwues.html

[R68] 计算文件校验值
来源：http://hz.daria6918.cn/gtdxzwrlzd.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.yuanzhike.top/gtqlujdmqd.html

[R69] 生成随机密码
来源：http://hz.c1oappe.top/gtpuiajlmr.html

head -c 16 /dev/urandom | base64
来源：http://hz.ydzc1.top/gtqeedjtfd.html

[R70] 时间戳与互转
来源：http://hz.yongpay.top/gtapvgbvqp.html

date +%s;  date -d @1700000000
来源：http://hz.yangfankeji.com/gtbbzjpeqp.html

[R71] 日期格式化
来源：http://hz.sweek.top/gtmqplyoui.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.ehwqpu.com/gtrlerellc.html

[R72] 等待端口就绪
来源：http://hz.52xcode.cn/gthyvswgmc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.zhiwuduotai.top/gtcfqkzzvf.html

[R73] 分割大日志
来源：http://hz.gotoacloud.top/gtgrhnyuwn.html

split -l 1000 big.log part_
来源：http://hz.iojbl.cn/gtruufuhcs.html

[R74] 批量重命名
来源：http://hz.52xcode.cn/gtsdkmfgbf.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.haohaochexian.top/gtotplynjl.html

[R75] 导出环境变量
来源：http://hz.zhengqikj.top/gtvvwzspag.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.dianchejie.cn/gtinebggjh.html

[R76] 使用临时文件
来源：http://hz.xingfuxueyuan.xyz/gtkrqtdklc.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.havefunace.top/gtxamyznap.html

[R77] 读取用户输入
来源：http://hz.yj202588.top/gteilapamq.html

read -rp "请输入: " ans
来源：http://hz.cqqwz.cn/gtjiiqmcvv.html

[R78] 交互式菜单
来源：http://hz.zhengqikj.top/gtjkmchuqr.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.c1oappe.top/gtykjufiwm.html

[R79] 解析命令行选项
来源：http://hz.bjfxy.top/gttxkemyax.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.wangshuangyany.cn/gtzhoislkf.html

[R80] 查看脚本执行耗时
来源：http://hz.guannengcc.top/gtfnlfirgc.html

time ./run.sh
来源：http://hz.ehwqpu.com/gtfvsjsitu.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtkfmqljll.html

S. C / C++ 专题
来源：http://hz.jlsjyb.cn/gtvsokkqpd.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtgwrzbgju.html

[S01] C：Hello World
来源：http://hz.mhx1999.top/gtbtktbusd.html

#include <stdio.h>
来源：http://hz.guannengcc.top/gtcheoxugo.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.yj202588.top/gtwfsbvexw.html

[S02] C：变量与格式化输出
来源：http://hz.yonumen.top/gtulrquwco.html

int a = 10; printf("%d\n", a);
来源：http://hz.zhengqikj.top/gtszmzkhgp.html

[S03] C：读入整数
来源：http://hz.jinyuanbaomall.cn/gttobndfps.html

int x; scanf("%d", &x);
来源：http://hz.zhaomingkeji.xyz/gtgepdlepz.html

[S04] C：字符串复制
来源：http://hz.zhengqikj.top/gtkpnhzhvl.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.guannengcc.top/gtqerseuqt.html

[S05] C：字符串长度
来源：http://hz.jinyuanbaomall.cn/gtumwcpqtx.html

strlen(s)
来源：http://hz.vqdsnc.cn/gtlpatqzeo.html

[S06] C：字符串比较
来源：http://hz.tianlin.xyz/gtjshtwivw.html

strcmp(a, b) == 0
来源：http://hz.xingfuxueyuan.xyz/gtjutnfrli.html

[S07] C：数组遍历求和
来源：http://hz.fzhhl.top/gttbsuzzxw.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.zhixingplan.top/gtrocjyowm.html

[S08] C：动态内存分配与释放
来源：http://hz.jqgfzy.top/gtulibfbxe.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.xziqi.cn/gtsjbrxgcc.html

[S09] C：结构体定义与初始化
来源：http://hz.0kj1m.cn/gtkavcekwu.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.jinyuanbaomall.cn/gtxjekfcur.html

[S10] C：指针与解引用
来源：http://hz.zhoulong.xyz/gtlilyznku.html

int *p = &a;  *p = 5;
来源：http://hz.jinghuilouyu.cn/gtemucgvxn.html

[S11] C：逐行读文件
来源：http://hz.dianchejie.cn/gtjkmfjrjq.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.redwolf501.top/gtntlsxtqv.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.yuanzhike.top/gtzcigpfqj.html

fclose(f);
来源：http://hz.yongpay.top/gtvxeobgkn.html

[S12] C：写文件
来源：http://hz.jinqigfzy.top/gtexikrxqg.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.gaohongyu789.top/gtoqxxsjnq.html

[S13] C：宏定义
来源：http://hz.feifeiyinyue.top/gtabgqmmes.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.jyoumei.cn/gtrirlatvg.html

[S14] C：枚举
来源：http://hz.fzhhl.top/gttauibldv.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.ybcxt.top/gttvkilwic.html

[S15] C：类型转换
来源：http://hz.quarkkingdee.top/gtcefabusj.html

(double) a / b
来源：http://hz.sweek.top/gtbjfaogtr.html

[S16] C：位操作置位
来源：http://hz.guowangkeji.top/gtvyowlmaa.html

x |= (1 << 3);
来源：http://hz.jinghuilouyu.cn/gtwqqrbibs.html

[S17] C：安全拼接字符串
来源：http://hz.meibo888.top/gtbotvbalo.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.xingfuxueyuan.xyz/gtjtabzwfd.html

[S18] C：命令行参数
来源：http://hz.jyoumei.cn/gtujtcvduk.html

int main(int argc, char **argv)
来源：http://hz.gotoacloud.top/gtoaaibstl.html

[S19] C：快速排序
来源：http://hz.yj20258.top/gtmhvavceg.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.iojbl.cn/gtvucunizu.html

[S20] C：二分查找
来源：http://hz.xuetiantiany.cn/gtcekrcjhb.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.jqgfzy.top/gtgzvfioge.html

[S21] C：字符类别判断
来源：http://hz.ydzc1.top/gtwugycysg.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.yangfankeji.com/gtxxdwvhxs.html

[S22] C：字符串转数字
来源：http://hz.nanxuanxn.top/gtmdsalhyf.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.sysykeji.top/gtssqecizd.html

[S23] C：随机数
来源：http://hz.yongpay.top/gtycyyzfkw.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.zhongyouzk.top/gtmipjnysu.html

[S24] C：获取本地时间
来源：http://hz.sysykeji.top/gtdfanehvu.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.dashuyun.cn/gtbgitqvaa.html

[S25] C：内存拷贝
来源：http://hz.zhoulong.xyz/gtxatrqbwu.html

memcpy(dst, src, n);
来源：http://hz.yj20258.top/gtnflzxgcz.html

[S26] C：内存清零
来源：http://hz.shangyingyoupin.top/gtsjvrhxgh.html

memset(a, 0, sizeof a);
来源：http://hz.andypj.xyz/gtibmwjldv.html

[S27] C：定义常量
来源：http://hz.jqgufenzy.top/gtwwdweiwg.html

const double PI = 3.14159;
来源：http://hz.c1oappe.top/gtbbstzuav.html

[S28] C：静态变量
来源：http://hz.dianchejie.cn/gtfvmcmkqf.html

static int counter = 0;
来源：http://hz.iojbl.cn/gtwtzlweac.html

[S29] C：变参函数
来源：http://hz.fengsongda.top/gtaxgutyil.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.zhiwuduotai.top/gtezsogkel.html

[S30] C：头文件保护
来源：http://hz.yuanzhike.top/gttfbhpxrp.html


<!-- 参考信息 -->