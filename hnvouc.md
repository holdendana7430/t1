代发 wailian999

[Q63] 开启事务
来源：http://hz.meibo888.top/gtwgcjnzwo.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.chenzaomai.com/gthjiuqpgu.html

[Q64] 提交事务
来源：http://hz.dianchejie.cn/gtronxmwik.html

COMMIT;
来源：http://hz.svipenyu.cn/gthkfaokoy.html

[Q65] 回滚事务
来源：http://hz.haohaochexian.top/gtbiwncouf.html

ROLLBACK;
来源：http://hz.andypj.xyz/gtorfxvhdv.html

[Q66] 行锁查询
来源：http://hz.daxiang520.top/gtrsrvfqxd.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.haohaochexian.top/gtqdsprtwy.html

[Q67] 设置隔离级别
来源：http://hz.yj20258888.top/gtjozdonaf.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.cdnleiting.top/gtqfwokmrx.html

[Q68] 保存点
来源：http://hz.pengpengdd.cyou/gtuackcoxe.html

SAVEPOINT sp1;
来源：http://hz.guannengcc.top/gtluqjxloi.html

ROLLBACK TO sp1;
来源：http://hz.yongpay.top/gthzwwrgjp.html

[Q69] 查看执行计划
来源：http://hz.cucudq.cn/gtdzixdqrb.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.pengpengdd.cyou/gtcmbajhru.html

[Q70] 更新统计信息
来源：http://hz.yueranfly.top/gtxxzbjmbv.html

ANALYZE TABLE users;
来源：http://hz.c1oappe.top/gttuomibcn.html

[Q71] 查看建表语句
来源：http://hz.aibaodan.cn/gtskfzvdyr.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.yj20258888.top/gtzkuwxbts.html

[Q72] 查看索引
来源：http://hz.shzxlz.cn/gtyvvqssdp.html

SHOW INDEX FROM users;
来源：http://hz.hywenlv.cn/gtsbzbnlii.html

[Q73] 查看表状态
来源：http://hz.yj202588.top/gthmfrxjhp.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.shanyushiyangtech.top/gtqiehouft.html

[Q74] 强制使用索引
来源：http://hz.yueranfly.top/gtgndoophg.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.mhx1999.top/gtjypfqovr.html

[Q75] 日期格式化
来源：http://hz.jinqigufen.top/gtqubmtoqb.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.vqdsnc.cn/gtirzbeouz.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.yj20258888.top/gtsgfzhbon.html

[Q76] 按天统计
来源：http://hz.dianchejie.cn/gtkxipdvps.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.xziqi.cn/gthyumwhth.html

[Q77] 时间加减
来源：http://hz.guannengcc.top/gtaijrxhxu.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.ybcxt.top/gtrogwuend.html

[Q78] 当前时间
来源：http://hz.yangfankeji.com/gtfdubpoxc.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.cucudq.cn/gtoinxnoyj.html

[Q79] 字符串拼接
来源：http://hz.52xcode.cn/gtqkirpqqq.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.ydjk.org.cn/gtentgjeph.html

[Q80] 字符串截取
来源：http://hz.feifeiyinyue.top/gtisxxhuro.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.yongpay.top/gtdppkfgnp.html

[Q81] 字符串替换
来源：http://hz.jlsjyb.cn/gtvhsqpxso.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.ehwqpu.com/gtrrjzvouw.html

[Q82] 字符长度与字节长度
来源：http://hz.yuanzhike.top/gtbsxsltja.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.ppjwa.cn/gtoisjuuwb.html

[Q83] 大小写转换
来源：http://hz.ybcxt.top/gtpqoburwx.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.ydzc1.top/gtdacaatob.html

[Q84] 去除首尾空格
来源：http://hz.yj202588.top/gtvupdorsw.html

SELECT TRIM(name) FROM users;
来源：http://hz.316326.xyz/gteuyudvje.html

[Q85] 数值取整
来源：http://hz.svipenyu.cn/gtvxkeancw.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.hammf.cn/gtaolbfmhh.html

[Q86] 读取 JSON 字段
来源：http://hz.cashguo.top/gtkcjkviva.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.guannengcc.top/gtkuiapkhd.html

[Q87] JSON 字段做条件
来源：http://hz.aibaodan.cn/gtgdnyputx.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.cheryme.top/gtbokjyjxd.html

[Q88] 行转列（条件聚合）
来源：http://hz.iojbl.cn/gtojubqiva.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.hongshengwenyu.top/gtstthgzqz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.cucudq.cn/gtcxritdtd.html

[Q89] 判断表是否存在
来源：http://hz.tianlin.xyz/gtqmjtmiiu.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.nanxuanxn.top/gteetjeqaf.html

[Q90] 生成序号列
来源：http://hz.zhiwuduotai.top/gtikqfymst.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.zhiwuduotai.top/gtdhzoyrou.html

================================================================================
来源：http://hz.bjfxy.top/gtpqydblft.html

R. Bash 专题
来源：http://hz.mhx1999.top/gtcnqqtsae.html

================================================================================
来源：http://hz.birdmap.top/gtzniqscdh.html

[R01] shebang 与严格模式
来源：http://hz.shanyushiyangtech.top/gtdllfupqo.html

#!/usr/bin/env bash
来源：http://hz.zhongyouzk.top/gtcsznkhtq.html

set -euo pipefail
来源：http://hz.jinqigfzy.top/gtektopdpk.html

[R02] 变量赋值与使用
来源：http://hz.xingfuxueyuan.xyz/gtrwaqvjxo.html

name="Tom"; echo "$name"
来源：http://hz.zycfv.cn/gtkxuileje.html

[R03] 只读变量
来源：http://hz.havefunace.top/gtffvokrqo.html

readonly PI=3.14
来源：http://hz.jinghuilouyu.cn/gtrdhjvkdg.html

[R04] 位置参数
来源：http://hz.zhijiandao.cn/gtbjnsiwsw.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.xylfe.cn/gtpadxiufd.html

[R05] 参数默认值
来源：http://hz.52xcode.cn/gtyvehdbzz.html

name="${1:-default}"
来源：http://hz.redwolf501.top/gtbwmmielh.html

[R06] 判断命令是否存在
来源：http://hz.yueranfly.top/gtmsclvljx.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.jqgfzy.top/gtrthnfjoo.html

[R07] if 判断文件
来源：http://hz.zdqjudy.top/gtafteqpyg.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.tian-w.cn/gtrffddsiy.html

[R08] 数值比较
来源：http://hz.haohaochexian.top/gtyjclhncn.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.wangshuangyany.cn/gttkyptwam.html

[R09] 字符串比较
来源：http://hz.tianlin.xyz/gtssbjauup.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.zhaomingkeji.xyz/gtrkodrdjz.html

[R10] 正则匹配
来源：http://hz.bjfxy.top/gtexoxpqdk.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.yonumen.top/gttuiiqams.html

[R11] case 多分支
来源：http://hz.gzhubu.top/gthzxpxrnf.html

case "$1" in
来源：http://hz.yuanzhike.top/gtozrkwedr.html

start) echo "启动" ;;
来源：http://hz.nanxuanxn.top/gtrkddbwnm.html

stop)  echo "停止" ;;
来源：http://hz.yj20258.top/gthjjsajax.html

*)     echo "未知命令" ;;
来源：http://hz.pycfn.com/gtwyjnhbqa.html

esac
来源：http://hz.haohaochexian.top/gtqzdyninu.html

[R12] for 遍历文件
来源：http://hz.gzhubu.top/gteezmuxpd.html

for f in *.txt; do echo "$f"; done
来源：http://hz.zhaomingkeji.xyz/gtldaplfmi.html

[R13] for 计数循环
来源：http://hz.yj20258.top/gtldmrqpzz.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.jlsjyb.cn/gtatzryewl.html

[R14] C 风格 for
来源：http://hz.daria6918.cn/gtrfbspkrl.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.jinghuilouyu.cn/gtsdgdqrbw.html

[R15] while 逐行读文件
来源：http://hz.cheryme.top/gthiqygzdh.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.shanyushiyangtech.top/gtsmszujui.html

[R16] until 等待条件
来源：http://hz.hammf.cn/gttfonyteh.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.wangdashe.top/gttbospfeb.html

[R17] 数组定义与取值
来源：http://hz.haohaochexian.top/gtjgwiixuu.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.ehwqpu.com/gticghsubf.html

[R18] 遍历数组
来源：http://hz.zdqjudy.top/gtvlftsvxc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.xylfe.cn/gtvgxqfpob.html

[R19] 数组长度
来源：http://hz.xziqi.cn/gtznmkxapa.html

echo "${#arr[@]}"
来源：http://hz.shzxlz.cn/gtojmpaqgj.html

[R20] 关联数组（字典）
来源：http://hz.ppjwa.cn/gtorgnnlkl.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.shanyushiyangkeji.top/gteuqfwxvb.html

[R21] 字符串长度
来源：http://hz.52xcode.cn/gtpvkhyilr.html

echo "${#s}"
来源：http://hz.meibo888.top/gtdmkleplu.html

[R22] 截取子串
来源：http://hz.zhiwuduotai.top/gtpzmlzqpm.html

echo "${s:0:5}"
来源：http://hz.daria6918.cn/gtwdijytes.html

[R23] 字符串替换
来源：http://hz.gotoacloud.top/gtdvrknmnu.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.cucudq.cn/gtcmxnvsnr.html

[R24] 大小写转换
来源：http://hz.shuidangran.top/gtkiornuxf.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.cheryme.top/gtbhydiqsu.html

[R25] 去后缀 / 去前缀
来源：http://hz.yongpay.top/gtxinfhrgw.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.0kj1m.cn/gtibqfmucv.html

[R26] 命令替换
来源：http://hz.nwbrower.top/gtovgxydww.html

now=$(date +%F); echo "$now"
来源：http://hz.tianlin.xyz/gtyqqghvpx.html

[R27] 算术展开
来源：http://hz.9152youxi.cn/gthzennvom.html

echo $((1 + 2 * 3))
来源：http://hz.sweek.top/gtqbakpvan.html

[R28] 浮点运算
来源：http://hz.xuanzx.com/gtvhiebrfz.html

echo "scale=2; 10/3" | bc
来源：http://hz.ppjwa.cn/gtkqvdfzyg.html

[R29] 定义函数
来源：http://hz.yj20258888.top/gtindmvnhs.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.zhijiandao.cn/gtbgduzfvf.html

[R30] 函数返回状态码
来源：http://hz.sweek.top/gtxanzwfqx.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.xingfuxueyuan.xyz/gtsqwixjng.html

[R31] 局部变量
来源：http://hz.quarkkingdee.top/gtjtlavgmk.html

f() { local x=1; echo "$x"; }
来源：http://hz.hywenlv.cn/gtwondujre.html

[R32] 参数个数校验
来源：http://hz.yanxiufei.cn/gtuhrunrkf.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.hywenlv.cn/gtopkmcdxs.html

[R33] 捕获错误并提示行号
来源：http://hz.fengsongda.top/gtdtmbbsgv.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.shuidangran.top/gtfzjjwvcv.html

[R34] 退出时清理
来源：http://hz.gzhubu.top/gtknwuerrs.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.tianlin.xyz/gtzkhtzwqd.html

[R35] 后台执行并等待
来源：http://hz.ywan-chungtsiang.top/gtptfkrjhq.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.c1oappe.top/gtwgatlqek.html

[R36] 并发执行多个任务
来源：http://hz.birdmap.top/gtamfwpote.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.xziqi.cn/gtqasqwiqh.html

[R37] 把输出赋给变量
来源：http://hz.yangfankeji.com/gtrzeoembt.html

files=$(ls -1)
来源：http://hz.chenzaomai.com/gtxuuufkbl.html

[R38] 管道串联
来源：http://hz.iojbl.cn/gtdmlbgdfm.html

cat a.txt | grep -i error | wc -l
来源：http://hz.yangfankeji.com/gtqcuevuqk.html

[R39] 重定向标准输出与错误
来源：http://hz.tanke756.top/gttugriayg.html

cmd > out.log 2>&1
来源：http://hz.zhijiandao.cn/gtxpmmlsou.html

[R40] 追加写日志
来源：http://hz.9152youxi.cn/gtivrhshci.html

echo "log" >> out.log
来源：http://hz.ybcxt.top/gtxsdpvtsu.html

[R41] 丢弃输出
来源：http://hz.snrcjt.cn/gtkqasqtof.html

cmd >/dev/null 2>&1
来源：http://hz.yongpay.top/gtodhrtguv.html

[R42] 输入重定向
来源：http://hz.daria6918.cn/gtbbmhnqwy.html

wc -l < a.txt
来源：http://hz.52xcode.cn/gtdinillbt.html

[R43] 按名字查找文件
来源：http://hz.yuanzhike.top/gtmjsxqqdl.html

find . -name "*.log" -type f
来源：http://hz.chenzaomai.com/gtcncqlgze.html

[R44] 按修改时间查找
来源：http://hz.quarkkingdee.top/gthuvyyosh.html

find . -mtime -7 -type f
来源：http://hz.zhoulong.xyz/gtjkitopgu.html

[R45] 批量删除
来源：http://hz.daria6918.cn/gtpdmppkio.html

find . -name "*.tmp" -delete
来源：http://hz.meibo888.top/gtykugqijg.html

[R46] 递归替换文件内容
来源：http://hz.316326.xyz/gtjtkimeuc.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.hysaishi.cn/gtkiogtquj.html

[R47] sed 单行替换
来源：http://hz.shangyingyoupin.top/gtyngpmjew.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.jinyuanbaomall.cn/gtsvojimla.html

[R48] awk 取指定列
来源：http://hz.aibaodan.cn/gtgeplozsf.html

awk '{print $1, $3}' a.txt
来源：http://hz.cucudq.cn/gtorrihkup.html

[R49] awk 带条件
来源：http://hz.tianlin.xyz/gtxdsghhfo.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.gaohongyu789.top/gtqgrzybmm.html

[R50] awk 求和
来源：http://hz.zycfv.cn/gtanxazbkl.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.yuanzhike.top/gtdvjqmbbw.html

[R51] 排序去重取前几
来源：http://hz.haohaochexian.top/gtcewekqsu.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.shanyushiyangtech.top/gtjdrjjsvx.html

[R52] 统计行数
来源：http://hz.cheryme.top/gtbiwwqhot.html

wc -l a.txt
来源：http://hz.zhaomingkeji.xyz/gtxesafqib.html

[R53] 查看文件头与实时尾
来源：http://hz.daria6918.cn/gtjjnooxyk.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.pycfn.com/gtyglpenjd.html

[R54] 比较两个文件
来源：http://hz.hammf.cn/gtfdywiwyv.html

diff a.txt b.txt
来源：http://hz.hfpthk.cn/gtwsqjjzkq.html

[R55] 压缩与解压
来源：http://hz.yongpay.top/gtncfwzphj.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.dashuyun.cn/gtuisqlozc.html

[R56] 远程拷贝
来源：http://hz.chenlongwang.top/gtdeaciehr.html

scp file user@host:/path/
来源：http://hz.jinyuanbaomall.cn/gtaskiuhxb.html

[R57] 远程执行命令
来源：http://hz.jinqigufen.top/gtzsonhljx.html

ssh user@host 'uptime'
来源：http://hz.jinqigfzy.top/gtvvwmnpvv.html

[R58] 下载文件
来源：http://hz.shzxlz.cn/gtyclhsyhw.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.vqdsnc.cn/gtxcxstuud.html

[R59] 发 POST JSON
来源：http://hz.guannengcc.top/gtwmpfkzse.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.hywenlv.cn/gtbwfhjywn.html

[R60] 只看 HTTP 状态码
来源：http://hz.hongshengwenyu.top/gtcedqfqws.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.shuidangran.top/gtijmjmipb.html

[R61] 磁盘占用
来源：http://hz.xuanzx.com/gtkmwwdjka.html

df -h;  du -sh *
来源：http://hz.gaohongyu789.top/gtgrknsibt.html

[R62] 找最占空间的文件
来源：http://hz.hysaishi.cn/gtuocgvvdj.html

du -ah . | sort -rh | head -10
来源：http://hz.zhiwuduotai.top/gtowhpszoj.html

[R63] 内存与进程
来源：http://hz.yuxming.cn/gtpdanpxar.html

free -h;  ps aux | grep nginx
来源：http://hz.sweek.top/gtgtrlcujg.html

[R64] 结束进程
来源：http://hz.daxiang520.top/gtracmhazu.html

kill -9 $(pgrep -f app.py)
来源：http://hz.hfpthk.cn/gtnrnvyhal.html

[R65] 查看端口占用
来源：http://hz.aizwys.cn/gtbjknsuqj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.yuxming.cn/gtxqkltjte.html

[R66] 定时任务
来源：http://hz.zdqjudy.top/gtrsgpgjsf.html

crontab -e;  crontab -l
来源：http://hz.ydzc1.top/gtierkrmki.html

[R67] 生成随机十六进制串
来源：http://hz.316326.xyz/gtzpcftrgs.html

openssl rand -hex 16
来源：http://hz.zhoulong.xyz/gtzrkntgln.html

[R68] 计算文件校验值
来源：http://hz.zhaomingkeji.xyz/gtmqszlsve.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.tianlin.xyz/gtcivtlwgr.html

[R69] 生成随机密码
来源：http://hz.jianghu66.top/gtfdnkrmyi.html

head -c 16 /dev/urandom | base64
来源：http://hz.chenlongwang.top/gtyetzcahh.html

[R70] 时间戳与互转
来源：http://hz.xziqi.cn/gtcodtznig.html

date +%s;  date -d @1700000000
来源：http://hz.tianlin.xyz/gteiifforx.html

[R71] 日期格式化
来源：http://hz.dianchejie.cn/gtwwjsilau.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.yj20258.top/gtpkkmridu.html

[R72] 等待端口就绪
来源：http://hz.yuanzhike.top/gtiozcurls.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.kuanghao11.cn/gtgirdhfij.html

[R73] 分割大日志
来源：http://hz.cheryme.top/gthamqemqo.html

split -l 1000 big.log part_
来源：http://hz.ehwqpu.com/gtuqwsryyi.html

[R74] 批量重命名
来源：http://hz.yuanzhike.top/gtitqqhjko.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.jianghu66.top/gtmanssyun.html

[R75] 导出环境变量
来源：http://hz.sysykeji.top/gttkfoxxpc.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.tanke756.top/gthkqtrtyo.html

[R76] 使用临时文件
来源：http://hz.hammf.cn/gttnzasfhl.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.hongshengwenyu.top/gtjmgcshap.html

[R77] 读取用户输入
来源：http://hz.shangyingyoupin.top/gtqccillgs.html

read -rp "请输入: " ans
来源：http://hz.snrcjt.cn/gtuelyygyq.html

[R78] 交互式菜单
来源：http://hz.cheryme.top/gtojhmzadg.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.ywan-chungtsiang.top/gtbyafowaq.html

[R79] 解析命令行选项
来源：http://hz.jyoumei.cn/gtyetdaxfe.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.ydjk.org.cn/gtylrymxmz.html

[R80] 查看脚本执行耗时
来源：http://hz.hfpthk.cn/gtdvqilqoi.html

time ./run.sh
来源：http://hz.wangshuangyany.cn/gtioqtqbek.html

================================================================================
来源：http://hz.tian-w.cn/gtbluwtikv.html

S. C / C++ 专题
来源：http://hz.pengpengdd.cyou/gtdfuhixex.html

================================================================================
来源：http://hz.smart0.xyz/gtwfdshkfn.html

[S01] C：Hello World
来源：http://hz.cqqwz.cn/gtomfacgzr.html

#include <stdio.h>
来源：http://hz.smart0.xyz/gtgcmxopne.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.guannengcc.top/gtpjgkfldp.html

[S02] C：变量与格式化输出
来源：http://hz.jinghuilouyu.cn/gtoxlhlxqn.html

int a = 10; printf("%d\n", a);
来源：http://hz.shuidangran.top/gtsgabvcmv.html

[S03] C：读入整数
来源：http://hz.tian-w.cn/gtslxergaj.html

int x; scanf("%d", &x);
来源：http://hz.pycfn.com/gtsnxflzch.html

[S04] C：字符串复制
来源：http://hz.shzxlz.cn/gtsylivell.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.daxiang520.top/gtuowpzmod.html

[S05] C：字符串长度
来源：http://hz.shzxlz.cn/gtlgvywzay.html

strlen(s)
来源：http://hz.fengsongda.top/gtezvnfeog.html

[S06] C：字符串比较
来源：http://hz.hnqzz.top/gtqcimcbou.html

strcmp(a, b) == 0
来源：http://hz.quarkkingdee.top/gtocnaxlcd.html

[S07] C：数组遍历求和
来源：http://hz.yongpay.top/gtwjuccchi.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.haohaochexian.top/gtjxumwxzn.html

[S08] C：动态内存分配与释放
来源：http://hz.tian-w.cn/gtvlvksfhd.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.yonumen.top/gtzlwqwdba.html

[S09] C：结构体定义与初始化
来源：http://hz.hnxiangtu.top/gtdystpxro.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.nwbrower.top/gtjdzeoeva.html

[S10] C：指针与解引用
来源：http://hz.wangshuangyany.cn/gtbyuwvtab.html

int *p = &a;  *p = 5;
来源：http://hz.nwbrower.top/gtgzifveyj.html

[S11] C：逐行读文件
来源：http://hz.sysykeji.top/gtvfshnfpj.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.yueranfly.top/gtxwussfzv.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.ydjk.org.cn/gttcmgivyx.html

fclose(f);
来源：http://hz.jinqigufen.top/gtonltdqrm.html

[S12] C：写文件
来源：http://hz.gogol.net.cn/gtnylffedg.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.yonumen.top/gtrarbxxnr.html

[S13] C：宏定义
来源：http://hz.ppjwa.cn/gttqmjuaht.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.yanxiufei.cn/gtvvmdynmt.html

[S14] C：枚举
来源：http://hz.zycfv.cn/gtsteqwxnc.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.fengsongda.top/gtrwrweshg.html

[S15] C：类型转换
来源：http://hz.tanke756.top/gtdodindiy.html

(double) a / b
来源：http://hz.jiagoushi.top/gtcwrjcips.html

[S16] C：位操作置位
来源：http://hz.guowangkeji.top/gtjukluhdz.html

x |= (1 << 3);
来源：http://hz.chenzaomai.com/gtnupdhope.html

[S17] C：安全拼接字符串
来源：http://hz.cheryme.top/gtzerluula.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.xinyue.icu/gtzoesqpum.html

[S18] C：命令行参数
来源：http://hz.jinyuanbaomall.cn/gtjjidmftr.html

int main(int argc, char **argv)
来源：http://hz.tanke756.top/gtcdnlvted.html

[S19] C：快速排序
来源：http://hz.svipenyu.cn/gttqocwefl.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.shuidangran.top/gtrtnmmczr.html

[S20] C：二分查找
来源：http://hz.cheryme.top/gtchkkpqfi.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.ybcxt.top/gtuubyxtqo.html

[S21] C：字符类别判断
来源：http://hz.ywan-chungtsiang.top/gtlvjbfcox.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.sysykeji.top/gtfanwtqze.html

[S22] C：字符串转数字
来源：http://hz.zhaomingkeji.xyz/gtnznimzso.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.cheryme.top/gtwngonfci.html

[S23] C：随机数
来源：http://hz.xinyue.icu/gtmiqvcayh.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.xziqi.cn/gtmdlquxyf.html

[S24] C：获取本地时间
来源：http://hz.316326.xyz/gtbrynfpeg.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.cucudq.cn/gtekgnrlfs.html

[S25] C：内存拷贝
来源：http://hz.hnxiangtu.top/gthohgikhx.html

memcpy(dst, src, n);
来源：http://hz.guowangkeji.top/gtjpirugak.html

[S26] C：内存清零
来源：http://hz.zhijiandao.cn/gtmkrurqxr.html

memset(a, 0, sizeof a);
来源：http://hz.zdqjudy.top/gterrgtcod.html

[S27] C：定义常量
来源：http://hz.hywenlv.cn/gtiataxwjf.html

const double PI = 3.14159;
来源：http://hz.316326.xyz/gtwbnwhohs.html

[S28] C：静态变量
来源：http://hz.jqgfzy.top/gteflsuoch.html

static int counter = 0;
来源：http://hz.yuxming.cn/gtnlfientx.html

[S29] C：变参函数
来源：http://hz.tianlin.xyz/gtnzowfqzx.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.gaohongyu789.top/gtrzpzzqte.html

[S30] C：头文件保护
来源：http://hz.sufxvd.cn/gtijxhnrlb.html

#ifndef X_H
来源：http://hz.yanxiufei.cn/gtulpxuczm.html

#define X_H
来源：http://hz.chenjidiqi.icu/gtkgiorxha.html

#endif
来源：http://hz.jinqigfzy.top/gtmolgrvou.html

[S31] C++：Hello World
来源：http://hz.ydzc1.top/gtqtyatsaw.html

#include <iostream>
来源：http://hz.xingfuxueyuan.xyz/gtnfnctkif.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.daria6918.cn/gtsfbakwew.html

[S32] C++：字符串
来源：http://hz.feifeiyinyue.top/gtaruqtxbi.html

std::string s = "hi";  s += "!";
来源：http://hz.pycfn.com/gtaadbssmk.html


<!-- 参考信息 -->