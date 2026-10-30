代发 wailian999

[Q80] 字符串截取
来源：http://www.share.zdbjq.cn/Article/details/gfrjnwerm.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fehbvm.com/Article/details/gidttgrqo.sHtML

[Q81] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/gdezucbxl.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fehbvm.com/Article/details/gybwaoyfc.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fehbvm.com/Article/details/gknmwobvc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gjshravcj.sHtML

[Q83] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/gwvssmhlv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gfbouuszp.sHtML

[Q84] 去除首尾空格
来源：http://m.share.zdbjq.cn/Article/details/gbwqvqoqj.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/getyqbprz.sHtML

[Q85] 数值取整
来源：http://blog.zdbjq.cn/Article/details/guihpcfij.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fehbvm.com/Article/details/gjvbovotx.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fehbvm.com/Article/details/glivwgtnw.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.zdbjq.cn/Article/details/gtiergxgx.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fehbvm.com/Article/details/gulmznkyl.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.zdbjq.cn/Article/details/goajqhwfj.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.fehbvm.com/Article/details/gtohucbfy.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.hesvh.cn/Article/details/gedzrwhlf.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fehbvm.com/Article/details/ggjdfgxvp.sHtML

[Q89] 判断表是否存在
来源：http://mobile.zdbjq.cn/Article/details/gamehtnej.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fehbvm.com/Article/details/gervmtepj.sHtML

[Q90] 生成序号列
来源：http://wap.zdbjq.cn/Article/details/gposiyoym.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.hesvh.cn/Article/details/gcyrjtvnh.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ghkgnhfcf.sHtML

R. Bash 专题
来源：http://www.share.zdbjq.cn/Article/details/gycejgcco.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gdpmfbisx.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fehbvm.com/Article/details/ggwqvhymy.sHtML

#!/usr/bin/env bash
来源：http://wap.fehbvm.com/Article/details/gvooktusi.sHtML

set -euo pipefail
来源：http://blog.fehbvm.com/Article/details/gicduhyqr.sHtML

[R02] 变量赋值与使用
来源：http://www.share.zdbjq.cn/Article/details/gvefuyvkl.sHtML

name="Tom"; echo "$name"
来源：http://m.share.zdbjq.cn/Article/details/gnghtogmp.sHtML

[R03] 只读变量
来源：http://3g.zdbjq.cn/Article/details/gewciwdud.sHtML

readonly PI=3.14
来源：http://www.blog.hesvh.cn/Article/details/gicefqftw.sHtML

[R04] 位置参数
来源：http://blog.zdbjq.cn/Article/details/gjvpgirpy.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.hesvh.cn/Article/details/gcqzxqpcp.sHtML

[R05] 参数默认值
来源：http://mobile.fehbvm.com/Article/details/gtwrwmhad.sHtML

name="${1:-default}"
来源：http://blog.zdbjq.cn/Article/details/gqsiveffy.sHtML

[R06] 判断命令是否存在
来源：http://blog.fehbvm.com/Article/details/gnqxlkjhi.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/gkagqxqzq.sHtML

[R07] if 判断文件
来源：http://blog.fehbvm.com/Article/details/gmtxzfmab.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fehbvm.com/Article/details/girfwrxhf.sHtML

[R08] 数值比较
来源：http://baike.zdbjq.cn/Article/details/gltyrxjqt.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fehbvm.com/Article/details/gipshzkgr.sHtML

[R09] 字符串比较
来源：http://3g.fehbvm.com/Article/details/gumjgxkke.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.zdbjq.cn/Article/details/geieswxyz.sHtML

[R10] 正则匹配
来源：http://www.share.fehbvm.com/Article/details/gcmafzigp.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.hesvh.cn/Article/details/gzzykauha.sHtML

[R11] case 多分支
来源：http://www.share.fehbvm.com/Article/details/gwmqcvziu.sHtML

case "$1" in
来源：http://www.blog.hesvh.cn/Article/details/gnisrbezg.sHtML

start) echo "启动" ;;
来源：http://www.share.hesvh.cn/Article/details/glakemjkl.sHtML

stop)  echo "停止" ;;
来源：http://blog.zdbjq.cn/Article/details/gsqbxenpy.sHtML

*)     echo "未知命令" ;;
来源：http://baike.zdbjq.cn/Article/details/gyfarhbbp.sHtML

esac
来源：http://wap.zdbjq.cn/Article/details/gjwejyxch.sHtML

[R12] for 遍历文件
来源：http://mobile.fehbvm.com/Article/details/gchcqilfi.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fehbvm.com/Article/details/gausfrjvd.sHtML

[R13] for 计数循环
来源：http://blog.zdbjq.cn/Article/details/gvryqitdz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/gdifiouod.sHtML

[R14] C 风格 for
来源：http://m.share.fehbvm.com/Article/details/gkycqsnym.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/grvutqglq.sHtML

[R15] while 逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gjaurjqgz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.hesvh.cn/Article/details/gxpdmlgeu.sHtML

[R16] until 等待条件
来源：http://www.blog.zdbjq.cn/Article/details/gmlqgzjbi.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gbpcxmxcw.sHtML

[R17] 数组定义与取值
来源：http://blog.zdbjq.cn/Article/details/gknvcoukb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.hesvh.cn/Article/details/glzmvwouz.sHtML

[R18] 遍历数组
来源：http://wap.fehbvm.com/Article/details/gwihngeuv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.zdbjq.cn/Article/details/guwrivvyc.sHtML

[R19] 数组长度
来源：http://www.share.zdbjq.cn/Article/details/gjvrcqrkx.sHtML

echo "${#arr[@]}"
来源：http://3g.zdbjq.cn/Article/details/gygxpvzdk.sHtML

[R20] 关联数组（字典）
来源：http://www.share.zdbjq.cn/Article/details/gdfgfnxdy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.zdbjq.cn/Article/details/gzqenvoyo.sHtML

[R21] 字符串长度
来源：http://m.share.zdbjq.cn/Article/details/gmixqlhca.sHtML

echo "${#s}"
来源：http://www.m.share.hesvh.cn/Article/details/gcfmngazj.sHtML

[R22] 截取子串
来源：http://baike.zdbjq.cn/Article/details/gtsrrtftr.sHtML

echo "${s:0:5}"
来源：http://baike.hesvh.cn/Article/details/gwzaejueq.sHtML

[R23] 字符串替换
来源：http://wap.fehbvm.com/Article/details/gyckzedto.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fehbvm.com/Article/details/gaglmgoxi.sHtML

[R24] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/gwmsueryh.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.hesvh.cn/Article/details/gdrxopvpy.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.hesvh.cn/Article/details/gsmvsfehp.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.zdbjq.cn/Article/details/ghwocpkfu.sHtML

[R26] 命令替换
来源：http://m.share.hesvh.cn/Article/details/gvsfbmrol.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.hesvh.cn/Article/details/ghxqydcys.sHtML

[R27] 算术展开
来源：http://blog.fehbvm.com/Article/details/gimdvnfwa.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fehbvm.com/Article/details/gkydjkjaa.sHtML

[R28] 浮点运算
来源：http://m.share.zdbjq.cn/Article/details/gkvtzsjik.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.zdbjq.cn/Article/details/gwpaiihmt.sHtML

[R29] 定义函数
来源：http://3g.hesvh.cn/Article/details/ggxtfgmnj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.hesvh.cn/Article/details/goxevmmdq.sHtML

[R30] 函数返回状态码
来源：http://wap.zdbjq.cn/Article/details/gdmrrpgix.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fehbvm.com/Article/details/gleybfqdf.sHtML

[R31] 局部变量
来源：http://www.share.zdbjq.cn/Article/details/gbvgmymky.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.hesvh.cn/Article/details/gwhubrpwb.sHtML

[R32] 参数个数校验
来源：http://read.share.zdbjq.cn/Article/details/gzcerzbzf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggummydmq.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fehbvm.com/Article/details/gblqflgpv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.zdbjq.cn/Article/details/ggathompu.sHtML

[R34] 退出时清理
来源：http://m.share.hesvh.cn/Article/details/gswkofkte.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/gkvehuneo.sHtML

[R35] 后台执行并等待
来源：http://www.share.zdbjq.cn/Article/details/gnxhywtbg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fehbvm.com/Article/details/gxisnsyyy.sHtML

[R36] 并发执行多个任务
来源：http://mobile.hesvh.cn/Article/details/gtrknndvd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fehbvm.com/Article/details/gyampkhhj.sHtML

[R37] 把输出赋给变量
来源：http://read.share.hesvh.cn/Article/details/gyzuimbsi.sHtML

files=$(ls -1)
来源：http://m.share.hesvh.cn/Article/details/gazducinz.sHtML

[R38] 管道串联
来源：http://www.share.hesvh.cn/Article/details/geusjodjp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fehbvm.com/Article/details/gkhgqjxlc.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fehbvm.com/Article/details/gxqfuswfn.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/ggqrszaiy.sHtML

[R40] 追加写日志
来源：http://m.share.hesvh.cn/Article/details/gxxvclmdr.sHtML

echo "log" >> out.log
来源：http://www.m.share.hesvh.cn/Article/details/gowpdqgin.sHtML

[R41] 丢弃输出
来源：http://m.share.zdbjq.cn/Article/details/gitbhywom.sHtML

cmd >/dev/null 2>&1
来源：http://blog.zdbjq.cn/Article/details/gmmaovmvx.sHtML

[R42] 输入重定向
来源：http://mobile.fehbvm.com/Article/details/gypsoeyio.sHtML

wc -l < a.txt
来源：http://mobile.hesvh.cn/Article/details/gdrrghvnk.sHtML

[R43] 按名字查找文件
来源：http://baike.zdbjq.cn/Article/details/gjfvtzdho.sHtML

find . -name "*.log" -type f
来源：http://blog.hesvh.cn/Article/details/gfpdcjyiz.sHtML

[R44] 按修改时间查找
来源：http://www.blog.zdbjq.cn/Article/details/gjmlbqjdm.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fehbvm.com/Article/details/gkpwvqtxc.sHtML

[R45] 批量删除
来源：http://baike.fehbvm.com/Article/details/gzmbxxckm.sHtML

find . -name "*.tmp" -delete
来源：http://baike.hesvh.cn/Article/details/gfcxrvcmt.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.zdbjq.cn/Article/details/gkljveqja.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.hesvh.cn/Article/details/gmykndmuc.sHtML

[R47] sed 单行替换
来源：http://baike.hesvh.cn/Article/details/gwfueqbgw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fehbvm.com/Article/details/gnocrblce.sHtML

[R48] awk 取指定列
来源：http://wap.fehbvm.com/Article/details/gzsdrrvbr.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.zdbjq.cn/Article/details/giyvmqqhf.sHtML

[R49] awk 带条件
来源：http://m.share.hesvh.cn/Article/details/gvxyqfamp.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.hesvh.cn/Article/details/glbpamtko.sHtML

[R50] awk 求和
来源：http://www.blog.fehbvm.com/Article/details/gsarhdqkz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gofbbpvec.sHtML

[R51] 排序去重取前几
来源：http://read.share.fehbvm.com/Article/details/gfvrkcgtz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.zdbjq.cn/Article/details/glfzvrdsj.sHtML

[R52] 统计行数
来源：http://www.share.zdbjq.cn/Article/details/gepsyurqa.sHtML

wc -l a.txt
来源：http://blog.zdbjq.cn/Article/details/gqcxrhpju.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.hesvh.cn/Article/details/gvhxqbbhp.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.zdbjq.cn/Article/details/gunljtxxx.sHtML

[R54] 比较两个文件
来源：http://www.share.zdbjq.cn/Article/details/gfgatvlss.sHtML

diff a.txt b.txt
来源：http://mobile.zdbjq.cn/Article/details/gtimcyukb.sHtML

[R55] 压缩与解压
来源：http://mobile.fehbvm.com/Article/details/gnlaasvnh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.hesvh.cn/Article/details/gcglpfvtm.sHtML

[R56] 远程拷贝
来源：http://m.share.zdbjq.cn/Article/details/gbdnufagb.sHtML

scp file user@host:/path/
来源：http://baike.zdbjq.cn/Article/details/gonfnmngh.sHtML

[R57] 远程执行命令
来源：http://wap.hesvh.cn/Article/details/gpsaqijzj.sHtML

ssh user@host 'uptime'
来源：http://wap.zdbjq.cn/Article/details/gnjtbxvav.sHtML

[R58] 下载文件
来源：http://baike.fehbvm.com/Article/details/gdycsmxnw.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.zdbjq.cn/Article/details/gwailvwcg.sHtML

[R59] 发 POST JSON
来源：http://3g.hesvh.cn/Article/details/gwhwhimff.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fehbvm.com/Article/details/gdhmmozfi.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fehbvm.com/Article/details/gvtfmqvne.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fehbvm.com/Article/details/gzncvfope.sHtML

[R61] 磁盘占用
来源：http://m.share.fehbvm.com/Article/details/gpckgpjks.sHtML

df -h;  du -sh *
来源：http://www.m.share.hesvh.cn/Article/details/ggrccfrrc.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fehbvm.com/Article/details/gfuenieox.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.hesvh.cn/Article/details/guwiomiig.sHtML

[R63] 内存与进程
来源：http://www.share.zdbjq.cn/Article/details/gtwjupbjr.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.hesvh.cn/Article/details/gcbofbjkv.sHtML

[R64] 结束进程
来源：http://read.share.hesvh.cn/Article/details/gsnjtsngj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.hesvh.cn/Article/details/ghswaozrf.sHtML

[R65] 查看端口占用
来源：http://3g.zdbjq.cn/Article/details/gjjhrngxi.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fehbvm.com/Article/details/gkjycckhu.sHtML

[R66] 定时任务
来源：http://www.share.hesvh.cn/Article/details/gmiitylbc.sHtML

crontab -e;  crontab -l
来源：http://wap.fehbvm.com/Article/details/gboinfqyz.sHtML

[R67] 生成随机十六进制串
来源：http://3g.zdbjq.cn/Article/details/gjzicbxug.sHtML

openssl rand -hex 16
来源：http://read.share.zdbjq.cn/Article/details/gkqjdlwsn.sHtML

[R68] 计算文件校验值
来源：http://wap.hesvh.cn/Article/details/gsazsqscp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fehbvm.com/Article/details/geoznvqvx.sHtML

[R69] 生成随机密码
来源：http://www.blog.fehbvm.com/Article/details/gitwolimt.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.zdbjq.cn/Article/details/gpivaniuz.sHtML

[R70] 时间戳与互转
来源：http://m.share.hesvh.cn/Article/details/gvspzpnaq.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fehbvm.com/Article/details/gtdiujach.sHtML

[R71] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/gpfsecoib.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.zdbjq.cn/Article/details/ggjhrvrmu.sHtML

[R72] 等待端口就绪
来源：http://wap.fehbvm.com/Article/details/gmmwvfqpa.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/gyjujmoys.sHtML

[R73] 分割大日志
来源：http://m.share.zdbjq.cn/Article/details/ghbkepjxa.sHtML

split -l 1000 big.log part_
来源：http://read.share.hesvh.cn/Article/details/gtaholghf.sHtML

[R74] 批量重命名
来源：http://blog.zdbjq.cn/Article/details/gvyuufpmj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.hesvh.cn/Article/details/gbpotfqks.sHtML

[R75] 导出环境变量
来源：http://3g.hesvh.cn/Article/details/gbvtamewb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.zdbjq.cn/Article/details/ghnimalct.sHtML

[R76] 使用临时文件
来源：http://m.share.zdbjq.cn/Article/details/gdsgychog.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/gommgyyld.sHtML

[R77] 读取用户输入
来源：http://wap.fehbvm.com/Article/details/gvdrhodet.sHtML

read -rp "请输入: " ans
来源：http://read.share.hesvh.cn/Article/details/gdiajavqx.sHtML

[R78] 交互式菜单
来源：http://blog.hesvh.cn/Article/details/gmpbpmuhi.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fehbvm.com/Article/details/gqpzjygnj.sHtML

[R79] 解析命令行选项
来源：http://3g.fehbvm.com/Article/details/gwcaqvkve.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.zdbjq.cn/Article/details/gmtfjctej.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.hesvh.cn/Article/details/gjlertbos.sHtML

time ./run.sh
来源：http://m.share.hesvh.cn/Article/details/gqyljahpd.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gjecatagl.sHtML

S. C / C++ 专题
来源：http://mobile.zdbjq.cn/Article/details/ggdasvqjx.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/golqhxjou.sHtML

[S01] C：Hello World
来源：http://read.share.fehbvm.com/Article/details/guctdxeyn.sHtML

#include <stdio.h>
来源：http://baike.hesvh.cn/Article/details/gphamsxxy.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.hesvh.cn/Article/details/ggmcckgsx.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.zdbjq.cn/Article/details/gimgfhxar.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.zdbjq.cn/Article/details/gthgvnfyh.sHtML

[S03] C：读入整数
来源：http://blog.fehbvm.com/Article/details/gcyrmzkgm.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fehbvm.com/Article/details/gdpficsry.sHtML

[S04] C：字符串复制
来源：http://3g.zdbjq.cn/Article/details/ggfyqqnjp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.zdbjq.cn/Article/details/gfzniijbj.sHtML

[S05] C：字符串长度
来源：http://baike.fehbvm.com/Article/details/gkmaimchf.sHtML

strlen(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gkpboyrqc.sHtML

[S06] C：字符串比较
来源：http://www.blog.fehbvm.com/Article/details/gplbhtbhg.sHtML

strcmp(a, b) == 0
来源：http://mobile.zdbjq.cn/Article/details/gmquamkxr.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fehbvm.com/Article/details/gmucgbcca.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.zdbjq.cn/Article/details/guduzmwmq.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fehbvm.com/Article/details/ggnmiudpy.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.zdbjq.cn/Article/details/ghacyfkux.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.zdbjq.cn/Article/details/gnpzvbebm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.zdbjq.cn/Article/details/gwbqffgfi.sHtML

[S10] C：指针与解引用
来源：http://wap.zdbjq.cn/Article/details/gcuueeciy.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fehbvm.com/Article/details/gmaindcqh.sHtML

[S11] C：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gnieujcmy.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.hesvh.cn/Article/details/gptjcoqsk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.zdbjq.cn/Article/details/gyxiafcid.sHtML

fclose(f);
来源：http://mobile.hesvh.cn/Article/details/giusaoitp.sHtML

[S12] C：写文件
来源：http://www.m.share.hesvh.cn/Article/details/grdzbhgad.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.zdbjq.cn/Article/details/gmmaspsof.sHtML

[S13] C：宏定义
来源：http://3g.fehbvm.com/Article/details/gdflttfxt.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.zdbjq.cn/Article/details/gflwlbnqg.sHtML

[S14] C：枚举
来源：http://mobile.fehbvm.com/Article/details/ggiskznxw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.hesvh.cn/Article/details/gprcdkebx.sHtML

[S15] C：类型转换
来源：http://m.share.fehbvm.com/Article/details/gxeqvbwyk.sHtML

(double) a / b
来源：http://blog.zdbjq.cn/Article/details/gnhdyzept.sHtML

[S16] C：位操作置位
来源：http://mobile.zdbjq.cn/Article/details/gpbkqzupt.sHtML

x |= (1 << 3);
来源：http://read.share.fehbvm.com/Article/details/gmopcnqxu.sHtML

[S17] C：安全拼接字符串
来源：http://blog.hesvh.cn/Article/details/gmwwilezc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fehbvm.com/Article/details/groozlirm.sHtML

[S18] C：命令行参数
来源：http://3g.fehbvm.com/Article/details/gstljzdrz.sHtML

int main(int argc, char **argv)
来源：http://wap.fehbvm.com/Article/details/ghcoraeum.sHtML

[S19] C：快速排序
来源：http://www.blog.hesvh.cn/Article/details/gdmidzgia.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/ggfpdhezh.sHtML

[S20] C：二分查找
来源：http://baike.fehbvm.com/Article/details/gmbyzgzez.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/gikcoylwh.sHtML

[S21] C：字符类别判断
来源：http://baike.hesvh.cn/Article/details/glahgtsih.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.zdbjq.cn/Article/details/gokokxcfb.sHtML

[S22] C：字符串转数字
来源：http://www.blog.hesvh.cn/Article/details/gkptdmapy.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.zdbjq.cn/Article/details/giivrrsnn.sHtML

[S23] C：随机数
来源：http://baike.fehbvm.com/Article/details/gragbmoxj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.hesvh.cn/Article/details/gldblphgb.sHtML

[S24] C：获取本地时间
来源：http://www.share.zdbjq.cn/Article/details/gsoxtzebh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.hesvh.cn/Article/details/gcoxcddgy.sHtML

[S25] C：内存拷贝
来源：http://baike.zdbjq.cn/Article/details/glntyjmib.sHtML

memcpy(dst, src, n);
来源：http://m.share.hesvh.cn/Article/details/ggmribtbl.sHtML

[S26] C：内存清零
来源：http://read.share.fehbvm.com/Article/details/gturvaudi.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.zdbjq.cn/Article/details/grertagce.sHtML

[S27] C：定义常量
来源：http://wap.zdbjq.cn/Article/details/gtdbxdwet.sHtML

const double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gnsdreykk.sHtML

[S28] C：静态变量
来源：http://wap.fehbvm.com/Article/details/gdlrigdyv.sHtML

static int counter = 0;
来源：http://blog.zdbjq.cn/Article/details/gugwvemvu.sHtML

[S29] C：变参函数
来源：http://www.blog.hesvh.cn/Article/details/gjydmsqhz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.zdbjq.cn/Article/details/gynpygvqr.sHtML

[S30] C：头文件保护
来源：http://blog.zdbjq.cn/Article/details/gbdzymiqu.sHtML

#ifndef X_H
来源：http://www.share.zdbjq.cn/Article/details/gbawfpgkf.sHtML

#define X_H
来源：http://www.share.fehbvm.com/Article/details/giotaruws.sHtML

#endif
来源：http://mobile.hesvh.cn/Article/details/gbsqzhhwg.sHtML

[S31] C++：Hello World
来源：http://www.share.fehbvm.com/Article/details/gckdkcwdx.sHtML

#include <iostream>
来源：http://read.share.hesvh.cn/Article/details/gqggwfumx.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.zdbjq.cn/Article/details/gfudjpoxx.sHtML

[S32] C++：字符串
来源：http://wap.fehbvm.com/Article/details/gewqviuqx.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.zdbjq.cn/Article/details/gsmxthqvd.sHtML

[S33] C++：vector 增删
来源：http://blog.zdbjq.cn/Article/details/gfghldses.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.hesvh.cn/Article/details/gcolueujq.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fehbvm.com/Article/details/gikajsmjo.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.hesvh.cn/Article/details/ginvuhtka.sHtML

[S35] C++：map
来源：http://3g.fehbvm.com/Article/details/gomeftldy.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gxlpytegr.sHtML

[S36] C++：unordered_map
来源：http://read.share.zdbjq.cn/Article/details/gnngbsczw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gqcyyczqf.sHtML

[S37] C++：set
来源：http://www.m.share.fehbvm.com/Article/details/gdsxqjfqj.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.hesvh.cn/Article/details/gpgzyeheb.sHtML

[S38] C++：排序
来源：http://baike.hesvh.cn/Article/details/gptnvqrys.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fehbvm.com/Article/details/gjxpwprrq.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fehbvm.com/Article/details/gbzlhvvoh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.hesvh.cn/Article/details/gbcnpskuk.sHtML

[S40] C++：查找元素
来源：http://www.blog.fehbvm.com/Article/details/gzihhhaxd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.hesvh.cn/Article/details/gvdphwiwq.sHtML

[S41] C++：类与构造函数
来源：http://m.share.hesvh.cn/Article/details/gbdgmnxln.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.hesvh.cn/Article/details/gmcutlrkq.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.hesvh.cn/Article/details/gemnxhkcw.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.zdbjq.cn/Article/details/gcrrdwdfw.sHtML

[S43] C++：智能指针
来源：http://baike.zdbjq.cn/Article/details/gpqwgfuxh.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.zdbjq.cn/Article/details/gelvfmtts.sHtML

[S44] C++：引用传参
来源：http://www.m.share.hesvh.cn/Article/details/geyvvedlb.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.zdbjq.cn/Article/details/gkmdbdbxx.sHtML

[S45] C++：lambda
来源：http://www.share.fehbvm.com/Article/details/ggbodumnt.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fehbvm.com/Article/details/gbwwwwtsr.sHtML

[S46] C++：函数模板
来源：http://wap.zdbjq.cn/Article/details/gkqrtxgqn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fehbvm.com/Article/details/goxxfwneo.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fehbvm.com/Article/details/giamxzqqn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.zdbjq.cn/Article/details/gsaglmzww.sHtML

[S48] C++：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gglppjmut.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.zdbjq.cn/Article/details/gyyrloedh.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.hesvh.cn/Article/details/gmpjhouwc.sHtML

[S49] C++：写文件
来源：http://mobile.zdbjq.cn/Article/details/gfxmwdlrz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.zdbjq.cn/Article/details/gbdetjtwx.sHtML

[S50] C++：格式化数字
来源：http://baike.fehbvm.com/Article/details/gmqgpyuse.sHtML


<!-- 参考信息 -->